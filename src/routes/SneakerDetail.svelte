<script>
    export let id;  // Este 'id' se pasa a través de la URL
  
    let sneaker = null;
  
    // Listado de zapatillas estáticas
    const sneakers = [
      { id: "nike-air-max", name: "Nike Air Max", image: "nike-air-max.jpg", description: "Descripción de las Nike Air Max", price: 120 },
      { id: "jordan-1", name: "Jordan 1", image: "jordan-1.jpg", description: "Descripción de las Jordan 1", price: 150 },
      { id: "nike-dunk", name: "Nike Dunk", image: "nike-dunk.jpg", description: "Descripción de las Nike Dunk", price: 110 },
      { id: "off-white", name: "Off-White", image: "off-white.jpg", description: "Descripción de las Off-White", price: 180 },
      { id: "adidas-ultraboost", name: "Adidas UltraBoost", image: "adidas-ultraboost.jpg", description: "Descripción de las Adidas UltraBoost", price: 130 },
      { id: "vans-old-skool", name: "Vans Old Skool", image: "vans-old-skool.jpg", description: "Descripción de las Vans Old Skool", price: 75 },
    ];
  
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
  