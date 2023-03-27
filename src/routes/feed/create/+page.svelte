<script>
    
    let author = "", title = "", text = "", attachments = "", major = "", tags = "";

    const handleSubmit = () => {
        fetch("http://localhost:2023/post", {
            method: "POST",
            headers: {
                'Content-Type': 'application/json',
                'Accept': 'application/json'
            },
            body: JSON.stringify({
                title : title,
                author: author,
                text  : text,
                major : major,
                tags  : tags,
                attachments: attachments,
            })
        })
        .then(res => res.json())
        .then(res => {
            console.log("Post POST result: ", res);
        });
    }
</script>



<h1>Create Opportunity Post</h1>

<form on:submit|preventDefault={handleSubmit} class="flex flex-col gap">
    <label for="title">title</label><input type="text" name="title" bind:value={title}/>
    <label for="author">author</label><input type="text" name="author" bind:value={author}/>
    <label for="text">text</label><input type="text" name="text" bind:value={text}/>
    <label for="attachments">attachments</label><input type="text" name="attachments" bind:value={attachments}/>
    <label for="major">major</label><input type="text" name="major" bind:value={major}/>
    <label for="tags">tags</label><input type="text" name="tags" bind:value={tags}/>


    <!-- author, title, text, attachments, major, tags -->
    <button type="submit">
        submit
    </button>
</form>


<style>
    input, button {
        @apply border;
    }
</style>