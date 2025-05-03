<template>
    <div class="cards">
      <nav>
        <h1 id="item">chevrolet onix</h1>
        <img :src="require('@/assets/veiculos-imagem/chevolet-onix.jpg')" alt="chevrolet-onix">
        <div class="card-descrição">
          <h2>Descrição</h2>
          <p>O Chevrolet Onix 2025 é um hatch compacto que combina design moderno, tecnologia avançada e segurança aprimorada, consolidando-se como um dos modelos mais populares do Brasil.</p>
          <button ref="a" >Saber Mais</button>
        </div>
      </nav>
    </div>
  </template>
  
<script>
export default {
    name: 'ChevroletOnixCard',
}
</script>