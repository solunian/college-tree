<script>
  import "../app.css";
  import Navbar from "$lib/components/Navbar.svelte";
</script>

<Navbar/>

<div class="flex flex-row justify-center w-full font-poppins">
  <main class="flex flex-col">
      <slot />
  </main>
</div>