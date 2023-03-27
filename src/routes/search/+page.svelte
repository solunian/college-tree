<script>
    import Post from "$lib/components/Post.svelte";
    const path = "http://localhost:2023";

    let tag = "";
    let feed = [];
    const handleOnSearch = async () => {
		const res = await fetch(path + `/search/${tag}`);
		feed = await res.json();
        console.log(feed);
    };
</script>

<div>
    {#if (feed === [])}
        {#each feed as post}
            <h>{post.title}</h>
            <Post post />
        {/each}
    {:else}
        <h2>Enter username:</h2>
        <form on:submit|preventDefault={handleOnSearch} class="flex flex-col gap">
            <input type="text" name="tag" bind:value={tag}/>
            <button type="search">
                search
            </button>
        </form>
    {/if}
    
</div>
