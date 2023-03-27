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
    <h1 class="text-3xl my-8">
        Search
    </h1>


    {#if (feed.length !== 0)}
        {#each feed as post}
            <Post {...post} />
        {/each}
    {:else}
        <h2>Tag to Search:</h2>
        <form on:submit|preventDefault={handleOnSearch} class="flex flex-col gap">
            <input type="text" name="tag" bind:value={tag}/>
            <button type="search">
                search
            </button>
        </form>
    {/if}
    
</div>


<style>
    input, button {
        @apply border;
    }
</style>