<template>
    <main>
        <div class="container-fluid">
            <div id="mainSlider" class="carousel slide" data-ride="carousel">
                <ol class="carousel-indicators">
                    <li data-bs-target="#mainSlider" data-bs-slide-to="0" class="active"></li>
                    <li data-bs-target="#mainSlider" data-bs-slide-to="1"></li>
                    <li data-bs-target="#mainSlider" data-bs-slide-to="2"></li>
                </ol>
                <div class="carousel-inner">
                    <div class="carousel-item active">

                        <img src="../assets/banner1.png" class="d-block w-100" alt="Projetos de E-commerce">
                        <div class="carousel-caption d-none d-md-block">

                            <h2>Quer criar um e-commerce?</h2>
                            <p>Conte conosco, temos mais de 30 lojas no portifólio</p>
                            <a href="#" class="main-btn">Ver portifólio</a>
                        </div>
                    </div>

                    <div class="carousel-item">
                        <img src="../assets/banner2.png" class="d-block w-100" alt="Engenhariade Software">
                        <div class="carousel-caption d-none d-md-block">
                            <h2>Esta querendo tirar o projeto do papel?</h2>
                            <p>Nossa equipe de engenharia de software esta pronta!</p>
                            <a href="#" class="main-btn">Entre em contato</a>
                        </div>
                    </div>

                    <div class="carousel-item">
                        <img src="../assets/banner3.png" class="d-block w-100" alt="Projetos Software">
                        <div class="carousel-caption d-none d-md-block">
                            <h2>Buscando manutenção?</h2>
                            <p>Temos profissionais altamente qualificados</p>
                            <a href="#" class="main-btn">Entre em contato</a>
                        </div>
                    </div>
                </div>
            </div>
            <Sobre/>
        </div>
    </main>
</template>

<style>

.container-fluid {
  padding-left: 0 !important;
  padding-right: 0 !important;
}
</style>

<script>
import Sobre from "./Sobre.vue"
export default {
    name: "ConteudoMain",

    components:{
        Sobre
    },

    data() {
        return {

        }
    }
}
</script>