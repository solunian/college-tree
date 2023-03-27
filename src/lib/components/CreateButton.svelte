<script>
    import plusIcon from "$lib/images/plus.svg";
    import { goto } from "$app/navigation";

    const createPostClickHandler = () => {
        goto("/feed/create");
    }
</script>


<button class="fixed bottom-5 right-5 w-12 h-12 text-5xl rounded-2xl outline outline-1 outline-gray-300 
p-2 hover:bg-purple-200 duration-200 ease-in-out" 
on:click={createPostClickHandler}>
    <img src={plusIcon} alt=""/>
</button>