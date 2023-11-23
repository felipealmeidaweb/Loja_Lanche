<template>
  <nav class="navbar navbar-expand-md" id="nav">
    <div class="container-fluid">
      <RouterLink to="/" class="navbar-brand">
        <img :src="logo" :alt="alt" class="w-33 h-25" style="width: 70px; height: 70px;">
      </RouterLink>

      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse text-center " id="navbarNavAltMarkup">
        <div class="navbar-nav m-auto">
          <RouterLink to="/" class="nav-link me-4">Home</RouterLink>
          <RouterLink to="/Pedidos" class="nav-link">Carrinho</RouterLink>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default{
  name:"NavBar",
  props:["logo","alt"]
}
</script>

<style scoped>

 #nav{
  background-color: #8C451C;
  
 }
 a {
  color: #18272F;
  position: relative;
  text-decoration: none;
}

a::before {
  content: '';
  position: absolute;
  width: 100%;
  height: 4px;
  border-radius: 4px;
  background-color: #ffffff;
  bottom: 0;
  left: 0;
  transform-origin: right;
  transform: scaleX(0);
  transition: transform .3s ease-in-out;
}

a:hover::before {
  transform-origin: left;
  transform: scaleX(1);
}
 /* Estilo para links ativos */
a:active {
  color: white;
}

/* Estilo para links visitados */
a:visited {
  color: white;
}
</style>