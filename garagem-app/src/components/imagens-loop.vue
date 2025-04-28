<template>
    <div class="imagens-loop">
        <div class="imagens-loop__container">
            <div id="imagens-loop__container">
                <img ref={{imagens}}> </img> 
            </div>
        </div>
    </div>
</template>
<script>
export default {
    name: 'ImagensLoop',
    data() {
        return {
            imagens: [],
            imagemAtual: 0,
            intervalo: null,
        };
    },
}
</script>