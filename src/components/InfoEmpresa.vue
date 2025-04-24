<template>
    <section class="container text-center mb-0">
        <div class="row">
            <h3 class="col-md-12 main-title">Entre em contato conosco</h3>

            <div class="col-md-4 contact-box">
                <i class="bi bi-telephone-fill"></i>
                <p><span class="alert-link">Ligue para: </span>(00) 00000-0000</p>
                <p><span class="alert-link">Horários: </span>08:00 - 19:00</p>
            </div>

            <div class="col-md-4 contact-box">
                <i class="bi bi-envelope-arrow-down-fill"></i>
                <p><span class="alert-link">Envie um e-mail: </span>contato@agencia.com</p>
            </div>

            <div class="col-md-4 contact-box">
                <i class="bi bi-geo-alt-fill"></i>
                <p><span class="alert-link">Venha nos conhecer: </span>Rua Jorge Henrique - 123</p>
            </div>
        </div>
    </section>
</template>

<style scoped>
.contact-box {
    padding-bottom: 50px;
    margin-bottom: 50px;
    border-bottom: 1px solid #3ec1d5;
}

.contact-box i {
    color: #444;
    border: 1px solid #444;
    border-radius: 50%;
    line-height: 55px;
    font-size: 24px;
    padding: 10px;
}

p {
    margin-top: 20px;
}
</style>

<script>
export default {
    name: "InfoEmpresa"
}
</script>