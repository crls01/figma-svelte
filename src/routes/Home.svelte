<script>
  import Navbar from "../components/Navbar.svelte";
</script>

<Navbar />

<h1>Ediciones limitadas</h1>
<div class="grid"></div>

<style>
  .grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 1rem;
    padding: 1rem;
  }
</style>
