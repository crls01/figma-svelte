<script>
  export let sneaker;
</script>

<div class="card">
  <img src={sneaker.image} alt={sneaker.name} />
  <h2>{sneaker.name}</h2>
  <p>{sneaker.description}</p>
  <p>Precio: ${sneaker.price}</p>
  <a href={`/sneaker/${sneaker.id}`} class="details-link">Ver detalles</a>
</div>

<style>
  .card {
    border: 1px solid #ccc;
    padding: 1rem;
    border-radius: 8px;
    text-align: center;
  }
  img {
    width: 100%;
    height: auto;
    border-radius: 8px;
  }
  .details-link {
    margin-top: 0.5rem;
    display: inline-block;
    padding: 0.5rem 1rem;
    background-color: black;
    color: white;
    border-radius: 4px;
    text-decoration: none;
  }
</style>
