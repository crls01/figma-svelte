<script>
  import Router from "svelte-spa-router";
  import Home from "./routes/Home.svelte";
  import SneakerDetail from "./routes/SneakerDetail.svelte";
  import Navbar from "./components/Navbar.svelte";
  import Footer from "./components/Footer.svelte";

  const routes = {
    "/": Home,
    "/sneaker/:id": SneakerDetail, // Mantienes el patrón dinámico para la página de detalle
  };
</script>

<main>
  <Navbar />
  <h1>Zapatillas exclusivas</h1>
  <Router {routes} />
  <Footer />
</main>
