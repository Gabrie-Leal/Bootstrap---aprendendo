<template>
    <div id="services-area">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <h3 class="main-title">Nossas Especialidades</h3>
                </div>

                <div class="col-md-4 service-box">
                    <i class="bi bi-phone"></i>
                    <h4>E-commerce</h4>
                    <p>Utilizamos o real poder dos dispositivos móveis, contruindo aplicativos nativos</p>
                </div>

                <div class="col-md-4 service-box">
                    <i class="bi bi-cart-check-fill"></i>
                    <h4>Aplicativos Nativos</h4>
                    <p>Temos plataforma própria de e-commerce, que se adapta a qualquer forma de negócio</p>
                </div>

                <div class="col-md-4 service-box">
                    <i class="bi bi-brush-fill"></i>
                    <h4>Designe Criativo</h4>
                    <p>Nossos designes são especialidados em UI/UX e também vasta experência no mercado de software</p>
                </div>

                <div class="col-md-4 service-box">
                    <i class="bi bi-google"></i>
                    <h4>Experts em SEO</h4>
                    <p>Com nosso serviço de marketing seu site será melhor posicionado no Google e venderá mais.</p>
                </div>

                <div class="col-md-4 service-box">
                    <i class="bi bi-person-raised-hand"></i>
                    <h4>Suporte 24/7</h4>
                    <p>Você sempre terá alguem da equipe disponível para suporte, em diferentes plataformas. (chat, email, skype)</p>
                </div>

                <div class="col-md-4 service-box">
                    <i class="bi bi-hdd-stack-fill"></i>
                    <h4>Experiência em servidores</h4>
                    <p>Garantimos uptime e também rápido tempo de resposta do seu site para o seu cliente.</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style>
.service-box{
    text-align: center;
    margin-bottom: 50px;;
}

.service-box i, h4{
    transition: .5s;
}

.service-box i {
    font-size: 36px;
    margin-bottom: 20px;
    color:#444;
}

.service-box h4{
    font-size: 24px;
    margin-bottom: 20px;
}

.service-box:hover > i, .service-box > h4{
    color:#65DAF9;
}
</style>

<script>
export default {
    name: "Especialidades",
}
</script>