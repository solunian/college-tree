<script>
    import Tag from "$lib/components/Tag.svelte";
    import placeholderImg from "$lib/images/placeholder.gif";

    export let title = "", author = "", text = "", major = "", attachments = "", tags = [];

    
    
</script>

<div class="flex flex-col py-2 px-2 border rounded-xl m-5 bg-slate-50">
    <h2>{title}</h2>
    <h3>{author}</h3>
    <p>{text}</p>
    <p>{major}</p>
    <a style="color: #00f" href={attachments}>{attachments}</a>
    <div class="flex flex-row gap-1 flex-wrap">
        {#each tags as tag}
            <Tag val={tag}/>
        {/each}
    </div>
</div>