<script>
  export let links = [
    { name: "Nike", href: "#" },
    { name: "Jordan 1", href: "#" },
    { name: "Jordan 4", href: "#" },
    { name: "Nike Dunk", href: "#" },
    { name: "Off-White", href: "#" },
  ];
</script>

<nav class="navbar">
  <h1>SNEAKVERSE</h1>
  <ul>
    {#each links as link}
      <li><a href={link.href}>{link.name}</a></li>
    {/each}
  </ul>
</nav>

<style>
 .navbar {
  display: flex;
  justify-content: space-between;
  padding: 1rem;
  background: black;
  color: white;
  width: 100%; 
  margin: 0; 
}
  ul {
    display: flex;
    list-style: none;
  }
  li {
    margin: 0 1rem;
  }
  a {
    text-decoration: none;
    color: white;
  }
</style>
