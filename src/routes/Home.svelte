<script>
  import Navbar from "../components/Navbar.svelte";
  import Footer from "../components/Footer.svelte";
  import SneakerCard from "../components/SneakerCard.svelte";
</script>

<Navbar />

<h1>Ediciones limitadas</h1>
<div class="grid">
  {#each sneakers as sneaker}
    <SneakerCard {sneaker} />
  {/each}
</div>
<Footer />

<style>
  .grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 1rem;
    padding: 1rem;
  }
</style>
