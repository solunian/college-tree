<script>
    let editing = false; // is editing the profile

    let username = "";
    const handleSubmitUsername = () => {
        // fetch();
        editing = true;
    };

    let bio = "", major = "", tags = "";
    const handleSaveChanges = () => {
        // fetch(); put?
        // goto();
        editing = false;
    };
</script>




<h1 class="text-3xl mb-5">
    Profile
</h1>

{#if (editing)}
    <h2 class="text-2xl">
        {username}
    </h2>
    <form on:submit|preventDefault={handleSaveChanges} class="flex flex-col gap">
        <label for="bio">bio</label><input type="text" name="bio" bind:value={bio}/>
        <label for="major">major</label><input type="text" name="major" bind:value={major}/>
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