<script>
  export let id;

  let sneaker = null;

  // Buscar la zapatilla según el id
  sneaker = sneakers.find((item) => item.id === id);
</script>

{#if sneaker}
  <div class="sneaker-detail">
    <img src={sneaker.image} alt={sneaker.name} />
    <h1>{sneaker.name}</h1>
    <p>Precio: ${sneaker.price}</p>
    <p>{sneaker.description}</p>
  </div>
{:else}
  <p>Cargando...</p>
{/if}

<style>
  .sneaker-detail {
    max-width: 600px;
    margin: 2rem;
    text-align: center;
  }
  img {
    width: 100%;
    border-radius: 8px;
  }
</style>
