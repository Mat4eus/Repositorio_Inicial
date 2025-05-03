<template>
    <div id="app">
        <topo/>
        <br><br><br><br><br><br><br><br><br>
        <h2 class="segundo-titulo">Lista de Veículos</h2>
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