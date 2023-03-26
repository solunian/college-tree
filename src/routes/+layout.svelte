<script>
  import "../app.css";
  import Navbar from "$lib/components/Navbar.svelte";
  import CreateButton from "$lib/components/CreateButton.svelte";
</script>



<div class="flex flex-col w-full font-poppins">
  <Navbar/>
  <div class="flex flex-row justify-center">
    <main class="flex flex-col">
        <slot />
    </main>
    <CreateButton/>
  </div>
</div>