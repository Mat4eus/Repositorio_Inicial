<template>
    <div id="app">
        <topo/>
        <h2>Lista de Veículos</h2>
        <h3>Carros</h3>
        <h4>Carros em Destaque</h4>
        <listaCarros/>
        <rodape/>
    </div>
</template>

<script>
import  rodape from './components/rodape.vue'; 
import listaCarros from './components/lista-carros.vue';
import topo from './components/head.vue';

export default {
    name: 'App',
    components: {
        listaCarros,
        topo,
        rodape,
    },
};

</script>