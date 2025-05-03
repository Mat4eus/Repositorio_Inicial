<template>
    <div id="app">
        <topo/>       
        <rodape/>
    </div>
</template>

<script>
import  rodape from './components/rodape.vue'; 
import topo from './components/head.vue';

export default {
    name: 'App',
    components: {
        topo,
        rodape,
    },
};

</script>