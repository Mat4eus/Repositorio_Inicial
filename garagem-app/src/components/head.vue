<template>
    <div>
        <header>
            <nav>
                <a class="logo" href="/">logo</a>
                <div class="mobile-menu" @click="toggleMenu">
                    <div class="line1"></div>
                    <div class="line2"></div>
                    <div class="line3"></div>
                </div>
                <ul class="nav-list" :class="{ active: isMenuOpen }">
                    <li><a href="/">Inicio</a></li>
                    <li><a href="/">Sobre</a></li>
                    <li><a href="/">Projetos</a></li>
                    <li><a href="/">Contatos</a></li>
                </ul>	
            </nav>
            <main> 
                <br><br><br>
                <listaCarros/>
            </main>
        </header>
    </div>
</template>

<script>

import listaCarros from './lista-carros.vue'; // Importa o componente de lista de carros

export default {
    name: 'head',
    components: {
        listaCarros, 
    },    
    data() {
        return {
            isMenuOpen: false, // Estado para controlar o menu
        };
    },
    methods: {
        toggleMenu() {
            const navList = this.$el.querySelector('.nav-list'); // Seleciona a lista de navegação
            const mobileMenu = this.$el.querySelector('.mobile-menu'); // Seleciona o menu móvel
            const activeClass = 'active';

            // Adiciona ou remove a classe 'active' na lista de navegação e no menu móvel
            navList.classList.toggle(activeClass);
            mobileMenu.classList.toggle(activeClass);

            // Chama a animação para os links
            this.animateLinks();
        },
        animateLinks() {
            const navLinks = this.$el.querySelectorAll('.nav-list li'); // Seleciona os links
            navLinks.forEach((link, index) => {
                link.style.animation = link.style.animation
                    ? ''
                    : `navLinkFade 0.5s ease forwards ${index / 7 + 0.3}s`; // Define a animação com atraso
            });
        },
    },
};
</script>

<style scoped>
/* Adicione estilos para o menu ativo */
.nav-list {
    display: none; /* Esconde o menu por padrão */
}
.nav-list.active {
    display: block; /* Mostra o menu quando ativo */
}
.mobile-menu.active .line1,
.mobile-menu.active .line2,
.mobile-menu.active .line3 {
    background-color: #000; /* Exemplo de estilo para o menu ativo */
}

/* Exemplo de animação */
@keyframes navLinkFade {
    from {
        opacity: 0;
        transform: translateX(-50px);
    }
    to {
        opacity: 1;
        transform: translateX(0);
    }
}
</style>