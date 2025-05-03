<template>
    <div id="app">
        <topo/>
        <br><br><br><br>
        <veiculo1/>
        
    </div>
</template>

<script>
import veiculo1 from './components/veiculos-assets/vhevolt-onix.vue';
import topo from './components/head.vue';

export default {
    name: 'App',
    components: {
        veiculo1,
        topo,
    },
};

</script>