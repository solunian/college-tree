<script>
    
    let author = "", title = "", text = "", attachments = "", major = "", tags = "";

    const handleSubmit = () => {
        // fetch();
        // goto()
    }
</script>



<h1>Create Opportunity Post</h1>

<form on:submit|preventDefault={handleSubmit} class="flex flex-col gap">
    <div class="flex flex-row"> 
    </div>
    <label for="title">title</label><input type="text" name="title" bind:value={title}/>
    <label for="author">author</label><input type="text" name="author" bind:value={author}/>
    <label for="text">text</label><input type="text" name="text" bind:value={text}/>
    <label for="attachments">attachments</label><input type="text" name="attachments" bind:value={attachments}/>
    <label for="major">major</label><input type="text" name="major" bind:value={major}/>
    <label for="tags">tags</label><input type="text" name="tags" bind:value={tags}/>


    <!-- author, title, text, attachments, major, tags -->
    <button type="submit">
        Submit
    </button>
</form>


<style>
    input, button {
        @apply border;
    }
</style>