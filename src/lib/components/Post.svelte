<script>
    import Tag from "$lib/components/Tag.svelte";
    import placeholderImg from "$lib/images/placeholder.gif";

    let title = "", author = "", text = "", major = "";
    
</script>

<div class="flex flex-col py-2 px-2 border rounded-xl m-5 bg-slate-50">
    <h2>{title}</h2>
    <h3>{author}</h3>
    <img src={placeholderImg} alt="" class="w-96 rounded-md"/>
    <p>{text}</p>
    <p>{major}</p>
    <div class="flex flex-row gap-1 flex-wrap">
        <Tag/><Tag/>
        <Tag/><Tag/>
        <Tag/><Tag/>
    </div>
</div>