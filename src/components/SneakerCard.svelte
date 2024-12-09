<script>
  export let sneaker;
</script>

<div class="card">
  <img src={sneaker.image} alt={sneaker.name} />
  <h2>{sneaker.name}</h2>
  <p>{sneaker.description}</p>
  <button>Ver detalles</button>
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
  button{
    margin-top: 0.5rem;
    padding: .5rem 1rem;
    background: black;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }
</style>
