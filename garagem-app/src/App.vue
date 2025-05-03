<template>
    <div id="app">
        <p>Olá, mundo!</p><br>
        <p>aqui inicializara o vue</p><br>
        <p>deus abencoe a patria</p><br>
        <nav>
            <ul>
                <li></li>
                <li></li>
                <li></li>
            </ul>
        </nav>
        
    </div>
</template>

<script>
import veiculo1 from './components/veiculo-1.vue';
export default {
    name: 'App',
    components: {
        veiculo1,
    },
};

</script>