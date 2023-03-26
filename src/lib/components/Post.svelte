<script>
    import Tag from "$lib/components/Tag.svelte";
    import placeholderImg from "$lib/images/placeholder.gif";
</script>

<div class="flex flex-col py-2 px-2 border rounded-xl m-5">
    <h2>Post Title</h2>
    <img src={placeholderImg} alt="" class="w-80 rounded-md"/>

    <div class="flex flex-row gap-1">
        <Tag/><Tag/>
        <Tag/><Tag/>
    </div>
</div>