<template>
    <div id="apply-area">
        <div class="container-fluid h-100">
            <div class="row h-100">
                <div class="col-md-6 apply-box" id="company-img"></div>

                <div class="col-md-6 apply-box" id="pattern-img">
                    <h4>Gosta de desafios?</h4>
                    <p>Temos várias posições abertas, entre elas: Software Engineer, UI/UX Designer, Project Manager e
                        mais.</p>
                    <p>Clique no botão abaixo e confira os benefícios e as posições em aberto.</p>
                    <p>Aqui você terá a chance de trabalhar com as melhores tecnologias e os profissionais mais
                        capacitados.</p>
                    <a href="#" class="btn btn-primary" id="apply-btn">Saiba Mais</a>
                </div>
            </div>
        </div>
    </div>
</template>

<style>
#apply-area {
    height: 100%;
    overflow: hidden;
}

#apply-area .container-fluid,
#apply-area .row {
    height: 100%;
}

#apply-area .apply-box {
    padding: 70px 30px;
    text-align: center;
}

#company-img {
    background-image: url('../assets/empresa.jpg');
    background-size: cover;
    background-position: center;
}

#pattern-img {
    background-size: cover;
}

#pattern-img h4,
#pattern-img p {
    color: #FFF;
}

#pattern-img h4 {
    margin-top: 8%;
    margin-bottom: 20px;
    text-transform: uppercase;
}

#pattern-img p {
    margin-bottom: 20px;
}

#apply-btn {
    display: block;
    height: auto;
    width: 180px;
    margin: 30px auto 0;
    background-color: transparent;
    border-color: #FFF;
    color: #FFF;
}

#apply-btn:hover {
    border-color: #65DAF9;
    background-color: #65DAF9;
    color: #000;
}
</style>

<script>
export default {
    name: "Trabalho",

    methods: {
        carregarImagens() {
            setTimeout(function () {
                $('#apply-area').parallax({ imageSrc: '/pattern.png' });
            }, 200);
        }
    },

    mounted() {
        this.carregarImagens();
    }
};
</script>