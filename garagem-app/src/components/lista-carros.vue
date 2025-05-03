<template>
    <div class="container-veiculos">
        <veiculo1 />
        <veiculo2 />
        <veiculo3 />
        <veiculo4 />
        <veiculo5 />
    </div>
</template>
<script>
    import veiculo5 from './veiculos-assets/mercedes-c180.vue';
    import veiculo4 from './veiculos-assets/lancer.vue';
    import veiculo3 from './veiculos-assets/ford-shelb.vue';
    import veiculo2 from './veiculos-assets/mazda-rx7.vue';
    import veiculo1 from './veiculos-assets/chevolet-onix.vue';
    export default {
        name: 'lista-carros',
        components: {
            veiculo5,
            veiculo4,
            veiculo3,
            veiculo2,
            veiculo1,
        },
    }
</script>