<template>
    <main class="container-fluid">
        <div id="mainSlider" class="carousel slide" data-bs-ride="carousel">
            <ol class="carousel-indicators list-unstyled">
                <li data-bs-target="#mainSlider" data-bs-slide-to="0" class="active"></li>
                <li data-bs-target="#mainSlider" data-bs-slide-to="1"></li>
                <li data-bs-target="#mainSlider" data-bs-slide-to="2"></li>
            </ol>

            <div class="carousel-inner">
                <div class="carousel-item active">
                    <img src="../assets/banner1.png" class="d-block w-100" alt="...">
                    <div class="carousel-caption d-none d-md-block">
                        <h2>Quer criar um e-commerce?</h2>
                        <p>Conte conosco, temos mais de 30 lojas no portifólio</p>
                    </div>
                </div>
                <div class="carousel-item">
                    <img src="../assets/banner2.png" class="d-block w-100" alt="...">
                    <div class="carousel-caption d-none d-md-block">
                        <h2>Esta querendo tirar o projeto do papel?</h2>
                        <p>Nossa equipe de engenharia de software esta pronta!</p>
                        <a href="#" class="main-btn">Entre em contato</a>
                    </div>
                </div>
                <div class="carousel-item">
                    <img src="../assets/banner3.png" class="d-block w-100" alt="...">
                    <div class="carousel-caption d-none d-md-block">
                        <h2>Buscando manutenção?</h2>
                        <p>Temos profissionais altamente qualificados</p>
                        <a href="#" class="main-btn">Entre em contato</a>
                    </div>
                </div>
            </div>

            <button class="carousel-control-prev" type="button" data-bs-target="#mainSlider" data-bs-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Anterior</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#mainSlider" data-bs-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Próximo</span>
            </button>
        </div>

        <Sobre />
        <Especialidades />
        <Dados />
        <ColaboradoresCards />
        <Trabalho />
        <Portifolio />
    </main>
</template>

<style scoped>
.container-fluid {
    padding-left: 0 !important;
    padding-right: 0 !important;
}

p {
    color: #ffff;
}
</style>

<script>
import Sobre from "./Sobre.vue"
import Especialidades from "./Especialidades.vue"
import Dados from "./Dados.vue"
import ColaboradoresCards from "./ColaboradoresCards.vue"
import Trabalho from "./Trabalho.vue"
import Portifolio from "./Portifolio.vue"

export default {
    name: "ConteudoMain",

    components: {
        Sobre, Especialidades, Dados, ColaboradoresCards, Trabalho, Portifolio
    },

    data() {
        return {

        }
    }
}
</script>