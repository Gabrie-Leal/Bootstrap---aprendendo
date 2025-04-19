<template>
    <div id="about-area">
        <div class="container">
            <div class="row">
              <div class="col-12"> 
                <h3 class="main-title">Sobre a hDC Agency</h3>
              </div>
              <div class="col-md-6">
                <img class="img-fluid" src="../assets/agencia.jpg" alt="Agência hDC">
              </div>
              <div class="col-md-6">
                <h3 class="about-title">Uma agência que pensa no futuro</h3>
                <p>Nossos projetos são adaptados ao cliente e seu propósito.</p>
                <p>Após a especificação do projetos os arquitetos de software definirão as melhores tecnologias para seu projeto.</p>
                <p>E nossos designers trabalharão na sua interface/layout para impulsionar o negócio.</p>
                <p>Veja outros diferenciais:</p>
                <ul id="about-list">
                  <li><i class="bi bi-check-lg"></i> Utilização de Machine Learning / AI</li>
                  <li><i class="bi bi-check-lg"></i> Layout responsivo para todos os dispositivos</li>
                  <li><i class="bi bi-check-lg"></i> Integração com diversos sistemas do mercado</li>
                  <li><i class="bi bi-check-lg"></i> Sistema de pagamento próprio</li>
                  <li><i class="bi bi-check-lg"></i> Desenvolvimento com metodologia ágil</li>
                </ul>
              </div>
            </div>
          </div>
      </div>
</template>

<style scoped>
.about-area{
    background-color: #F9F9F9;
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

.about-title{
    font-size: 17px;
    color:#444;
    text-transform: uppercase;
    font-weight: bold;
}

#about-list{
    list-style: none;
    padding-left: 0;
}

li{
    line-height: 30px;
}

i{
    color:#65DAF9;
    margin-right: 15px;

}
</style>

<script>
export default{
    name:"Sobre",
    
    data(){
        return{
            
        }
    }
}
</script>