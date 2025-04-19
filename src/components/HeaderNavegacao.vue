<template>
    <header>
        <div class="container" id="nav-container">
            <nav class="navbar navbar-expand-lg fixed-top">
                <a href="#" class="navbar-brand">
                    <img src="../assets/hdcagency_logo.svg" alt="HDC Agency" id="logo">
                    HDC Agency
                </a>
                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="navbar-links"
                    aria-controls="navbar-links" arial-expanded="false" aria-label="toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>

                <div class="collapse navbar-collapse justify-content-end" id="navbar-links">
                    <div class="navbar-nav">
                        <a class="nav-item nav-link" href="#" id="home-menu">Home</a>
                        <a class="nav-item nav-link" href="#" id="about-menu">Agência</a>
                        <a class="nav-item nav-link" href="#" id="services-menu">Serviços</a>
                        <a class="nav-item nav-link" href="#" id="team-menu">Time</a>
                        <a class="nav-item nav-link" href="#" id="portifolio-menu">Projetos</a>
                        <a class="nav-item nav-link" href="#" id="contact-menu">Contato</a>
                    </div>
                </div>
            </nav>
        </div>
    </header>
</template>

<style scoped>
header,
.navbar {
    background-color: #353d41;
}

#nav-container {
    padding-top: 0;
    padding-bottom: 0;
}

#logo {
    width: 75px;
}

.navbar-brand{
    padding: 0;
    color:#fff;
}

.navbar-brand:hover{
    color:#fff;
}

#navbar-links a{
    color:#fff;
}

#navbar-expand-lg .navbar-nav .nav-links{
    padding: 1rem .8rem;
}
</style>

<script>
export default {
    name: "HeaderNavegacao",

    data() {
        return {

        }
    },
}
</script>
