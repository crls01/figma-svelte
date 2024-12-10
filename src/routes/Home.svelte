<script>
  import SneakerCard from "../components/SneakerCard.svelte";

  // Listado de zapatillas (estáticas)
  const sneakers = [
    { id: "nike-air-max", name: "Nike Air Max", image: "nike-air-max.jpg", description: "Descripción de las Nike Air Max", price: 120 },
    { id: "jordan-1", name: "Jordan 1", image: "jordan-1.jpg", description: "Descripción de las Jordan 1", price: 150 },
    { id: "nike-dunk", name: "Nike Dunk", image: "nike-dunk.jpg", description: "Descripción de las Nike Dunk", price: 110 },
    { id: "off-white", name: "Off-White", image: "off-white.jpg", description: "Descripción de las Off-White", price: 180 },
    { id: "adidas-ultraboost", name: "Adidas UltraBoost", image: "adidas-ultraboost.jpg", description: "Descripción de las Adidas UltraBoost", price: 130 },
    { id: "vans-old-skool", name: "Vans Old Skool", image: "vans-old-skool.jpg", description: "Descripción de las Vans Old Skool", price: 75 },
  ];
</script>

<div class="sneaker-list">
  {#each sneakers as sneaker}
    <SneakerCard {sneaker} />
  {/each}
</div>

<style>
  .sneaker-list {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 1rem;
  }
</style>
