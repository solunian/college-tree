<script>
    import Post from "$lib/components/Post.svelte";
    const path = "http://localhost:2023";

    let username = "";
    let feed = [];
    const handleSubmitUsername = async () => {
		const res = await fetch(path + `/posts/${username}`);
		feed = await res.json();
    };
</script>

<div>
	{#each feed as post}
        <h>{post.title}</h>
        <Post />
    {:else}
        <h2>Enter username:</h2>
        <form on:submit|preventDefault={handleSubmitUsername} class="flex flex-col gap">
            <input type="text" name="username" bind:value={username}/>
            <button type=submit>
                submit
            </button>
        </form>
    {/each}
</div>
