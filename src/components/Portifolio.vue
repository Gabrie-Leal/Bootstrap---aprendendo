<template>
    <div class="portifolio-area">
        <div class="container">
            <div class="row">
                <div class="col-md-12">
                    <h3 class="main-title">Conheça nossos projetos</h3>
                </div>

                <div class="col-md-12" id="filter-btn-box">
                    <button class="btn btn-primary active" ref="btnTodos" id="all-btn" @click="todos()">Todos</button>
                    <button class="btn btn-primary" ref="btnDev" id="dev-btn" @click="dev()">Desenvolvimento</button>
                    <button class="btn btn-primary" ref="btnDsg" id="dsg-btn" @click="dsg()">Design</button>
                    <button class="btn btn-primary" ref="btnSeo" id="seo-btn" @click="seo()">SEO</button>
                </div>
                <img class="col-md-4 img-fluid" v-for="(projeto, index) in projetos" :key="index" :src="projeto" alt="">
            </div>
        </div>
    </div>
</template>

<style scoped>
#filter-btn-box {
    text-align: center;
    margin-bottom: 30px;
}

#filter-btn-box button {
    border-radius: 20px;
    background: transparent;
    color: #444;
    border: 1px solid#444;
    text-transform: none;
    margin:0 15px;
    min-width: 100px;
    width: auto;
    height: 40px;
    line-height: 40px;
    padding: 0 20px;
}

#filter-btn-box .active {
    border-color: #65DAF9;
    background-color: #65DAF9;
    color: #fff;
}

img {
    margin-bottom: 3px;
    animation: fadeOut .5s;
}
</style>

<script>
import proj1 from '../assets/proj1.jpg';
import proj2 from '../assets/proj2.jpg';
import proj3 from '../assets/proj3.jpg';
import proj4 from '../assets/proj4.jpg';
import proj5 from '../assets/proj5.jpg';
import proj6 from '../assets/proj6.jpg';

export default {
    data() {
        return {
            projetos: [proj1, proj2, proj3, proj4, proj5, proj6]
        };
    },
    methods: {
        todos() {
            this.projetos = [proj1, proj2, proj3, proj4, proj5, proj6];
            this.resetAtivos();
            this.$refs.btnTodos.classList.add("active");
        },
        dev() {
            const btnSelecionado = this.$refs.btnDev;

            if (btnSelecionado.classList.contains("active")) {
                btnSelecionado.classList.remove("active");
                this.todos();
            } else {
                this.resetAtivos();
                this.projetos = [proj2, proj5, proj6];
                btnSelecionado.classList.add("active");
            }
        },
        dsg() {
            const btnSelecionado = this.$refs.btnDsg;

            if (btnSelecionado.classList.contains("active")) {
                btnSelecionado.classList.remove("active");
                this.todos();
            } else {
                this.resetAtivos();
                this.projetos = [proj1, proj3, proj6];
                btnSelecionado.classList.add("active");
            }
        },
        seo() {
            const btnSelecionado = this.$refs.btnSeo;

            if (btnSelecionado.classList.contains("active")) {
                btnSelecionado.classList.remove("active");
                this.todos();
            } else {
                this.resetAtivos();
                this.projetos = [proj3, proj4];
                btnSelecionado.classList.add("active");
            }
        },
        resetAtivos() {
            this.$refs.btnTodos.classList.remove("active");
            this.$refs.btnDev.classList.remove("active");
            this.$refs.btnDsg.classList.remove("active");
            this.$refs.btnSeo.classList.remove("active");
        }
    }
}
</script>
