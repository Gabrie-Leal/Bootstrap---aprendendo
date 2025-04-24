<template>
  <div>
    <HeaderNavegacao/>
    <ConteudoMain/>
    <Novidades/>
    <InfoEmpresa/>
    <Rodape/>
  </div>
</template>

<script>
import HeaderNavegacao from "./components/HeaderNavegacao.vue"
import ConteudoMain from "./components/ConteudoMain.vue"
import Novidades from "./components/Novidades.vue"
import InfoEmpresa from "./components/InfoEmpresa.vue"
import Rodape from "./components/Rodape.vue"

export default {
  components: {
    HeaderNavegacao,
    ConteudoMain,
    Novidades,
    InfoEmpresa,
    Rodape
  }
}
</script>

<style>
* {
  font-family: "Roboto", sans-serif;
}

.row {
  margin: 0;
}
.container {
  padding: 70px 0;
}
p, li {
  color: #444;
  font-size: 20px;
}

.main-title{
    color:#444;
    margin: 0 0 65px 0;
    font-size: 40px;
    text-align: center;
    position: relative;
}

.main-title::after {
    content:"";
    border-top:2px solid #333;
    width:15%;
    position: absolute;
    top:60px;
    left:42.5%;
}

@media(max-width: 768px) {
  
  /* geral */
  .container {
    padding: 20px 0;
  }
  
  /* slider */
  #mainSlider .carousel-inner, #mainSlider .carousel-item {
    height: auto;
  }

  #mainSlider .carousel-caption h2 {
    font-size: 28px;
  }

  #mainSlider .carousel-caption p {
    font-size: 18px;
    margin-bottom: 40px;
  }

  .carousel-caption {
    left: 10%;
    right: 10%;
  }
  
  /* about */
  #about-area img {
    margin-top: 100px;
  }
  
  /* data */
  .circle-box div {
    padding: 0 10px;
  }

  #data-area p {
    font-size: 16px;
  }
  
  /* team */
  .card-title {
    font-size: 14px;
  }

  .card-text {
    font-size: 12px;
  }

  /* apply */
  #apply-area .apply-box {
    padding: 50px 25px;
  }

  /* news */
  #news-area p {
    width: 80%;
    margin-left: auto;
    margin-right: auto;
  }

  #email-input {
    width: 70%;
  }

  #call-area {
    margin-top: 30px;
  }

  #call-area .container {
    padding: 30px;
  }

  #call-area p, #call-area #call-btn {
    font-size: 16px;
  }

}

@media(max-width: 425px) {

  #mainSlider {
    margin-top: 90px;
  }

  #mainSlider .carousel-caption {
    top: 5%;
  }

  #mainSlider .carousel-caption h2 {
    font-size: 18px;
    margin-bottom: 40px;
  }

  #mainSlider .carousel-caption p {
    display: none;
  }

  .carousel-caption .main-btn {
    
    font-size: 14px;
  }

  /* about */
  .main-title {
    font-size: 30px;
  }

  #about-area img {
    margin-top: 0;
    margin-bottom: 30px;
  }

  /* data */
  .circle-box {
    width: 50%;
  }

  #team-area .col-md-3 {
    width: 50%;
    margin-bottom: 30px;
  }

  /* apply */
  #apply-area {
    height: auto;
  }

  #company-img {
    display: none;
  }

  /* filter */
  #portfolio-area .filter-btn {
    margin-bottom: 20px;
  }

  .project-box {
    width: 50%;
  }

  /* news */
  #news-area .main-title {
    font-size: 24px;
  }

  #news-area p {
    font-size: 16px;
  }

  #email-input {
    width: 80%;
  }

  #call-area p, #call-area #call-btn {
    font-size: 14px;
    letter-spacing: 0;
  }

  #call-area p, #call-area #call-btn {
    margin: 0;
    width: 50%;
  }

  /* contact */
  .contact-box {
    border: none;
    margin-bottom: 0;
  }
}

</style>