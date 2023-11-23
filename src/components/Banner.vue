<template>
    <div class="main-banner">
        <h1>FAÇA O SEU LANCHE LOKO </h1>
        
    </div>
</template>

<script>
export default{
    name:"Banner",
}

</script>



<style scoped>
.main-banner {
  background-image: url(" /img/Lanche.jpg");
  background-position: center; /* Centralize o plano de fundo */
  background-size: cover;
  height: 500px; /* Altura fixa em 500px */
  display: flex;
  align-items: center;
  justify-content: end; /* Centralize o texto verticalmente e horizontalmente */
  background-repeat: no-repeat;
}

h1 {
  color: white;
  font-size: 2em; /* Tamanho de fonte relativo */
  

  padding: 20px 40px;
}

/* Adicione regras de mídia para estilos específicos em tamanhos diferentes */
@media (max-width: 768px) {
  .main-banner {
    height: 300px; /* Ajuste para telas menores */
  }
}
</style>





