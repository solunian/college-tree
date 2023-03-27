<script>
    const path = "http://localhost:2023";
    let editing = false; // is editing the profile

    let username = "", bio = "", majors = "", tags = "";
    const handleSubmitUsername = () => {
        fetch(path + `/user/${username}`)
        .then(res => res.json())
        .then(res => {
            console.log("res from submit username: ", res);
            if (res.err) {
                console.log("none such user.");
                return;
            }

            username = res.name;
            bio = res.bio;
            majors = res.majors;
            tags = res.tags;
            
            console.log(res);
            editing = true;
        });
    };

    const handleSaveChanges = () => {
        fetch(path + `/user/edit/${username}`, {
            method: "POST",
            headers: {
                'Content-Type': 'application/json',
                'Accept': 'application/json'
            },
            body: JSON.stringify({
                name : username,
                bio : bio,
                majors : majors,
                tags  : tags,
            })
        })
        .then(res => res.json())
        .then(res => {
            console.log(res);
            editing = false;
        });
    };
</script>




<h1 class="text-3xl my-8">
    Profile
</h1>

{#if (editing)}
    <h2 class="text-2xl">
        {username}
    </h2>
    <form on:submit|preventDefault={handleSaveChanges} class="flex flex-col gap">
        <label for="bio">bio</label><input type="text" name="bio" bind:value={bio}/>
        <label for="majors">major</label><input type="text" name="majors" bind:value={majors}/>
        <label for="tags">tags</label><input type="text" name="tags" bind:value={tags}/>

        <!-- author, title, text, attachments, major, tags -->
        <button type="submit">
            save changes
        </button>
    </form>
{:else}
    <h2>Enter username to create or edit your profile:</h2>
    <form on:submit|preventDefault={handleSubmitUsername} class="flex flex-col gap">
        <input type="text" name="username" bind:value={username}/>
        <button type=submit>
            submit
        </button>
    </form>

{/if}


<style>
    input, button {
        @apply border;
    }
</style>