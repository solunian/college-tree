<script>
    import Tag from "$lib/components/Tag.svelte";
    import placeholderImg from "$lib/images/placeholder.gif";
</script>

<div class="flex flex-col w-80">
    <h2>Post Title</h2>
    <img src={placeholderImg} alt=""/>

    <div class="flex flex-row gap-1">
        <Tag/><Tag/>
        <Tag/><Tag/>
    </div>
</div>