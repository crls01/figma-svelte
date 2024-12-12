<script>
  import SneakerCard from "../components/SneakerCard.svelte";

  // Listado de zapatillas (estáticas)
  const sneakers = [
    {
      id: "nike-air-max",
      name: "Nike Air Max",
      image: "/imgs/air-jordan-1-high-dior-removebg.png",
      description: "Descripción de las Nike Air Max",
      price: 120,
    },
    {
      id: "jordan-1",
      name: "Jordan 1",
      image: "/imgs/goodelgoose-removebg.png",
      description: "Descripción de las Jordan 1",
      price: 150,
    },
    {
      id: "nike-dunk",
      name: "Nike Dunk",
      image: "/imgs/Gucci-GG-Sneaker.png",
      description: "Descripción de las Nike Dunk",
      price: 110,
    },
    {
      id: "off-white",
      name: "Off-White",
      image: "/imgs/Nike-Back-To-The-Future-2011.png",
      description: "Descripción de las Off-White",
      price: 180,
    },
    {
      id: "adidas-ultraboost",
      name: "Adidas UltraBoost",
      image: "/imgs/pngegg.png",
      description: "Descripción de las Adidas UltraBoost",
      price: 130,
    },
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
    grid-template-columns: repeat(auto-fill, minmax(300px, 2fr));
    gap: 1rem;
    width: 100%;
    max-width: 100%;
    overflow: hidden; /* Evita que se desborde el contenedor */
  }
</style>
