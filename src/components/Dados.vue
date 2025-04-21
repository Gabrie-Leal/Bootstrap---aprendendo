<template>
    <div class="data-area">
        <div class="container">
            <div class="row">
                <div class="col-md-3 circle-box">
                    <div id="circleA"></div>
                    <p>Projetos entregeues</p>
                </div>

                <div class="col-md-3 circle-box">
                    <div id="circleB"></div>
                    <p>Clientes felizes</p>
                </div>

                <div class="col-md-3 circle-box">
                    <div id="circleC"></div>
                    <p>Colaboradores</p>
                </div>

                <div class="col-md-3 circle-box">
                    <div id="circleD"></div>
                    <p>Cafezinhho</p>
                </div>
            </div>
        </div>
    </div>
</template>

<style>
.circle{
    padding:0 40px;
}

.progressbar-text{
    font-weight: bold;
    font-size:32px;
}

#data-area{
    color:#fff;
    text-align: center;
    font-size: 26px;
    margin-top:20px;
}
</style>

<script>
import ProgressBar from 'progressbar.js'

export default {
  name: "Dados",

  methods:{
    circulos(){
        let containerA = document.getElementById("circleA");
        let circleA = new ProgressBar.Circle(containerA, {
        color: "#64DAF9",
        strokeWidth: 8,
        duration: 1400,
        from: { color: '#aaa' },
        to: { color: '#65daf9' },

        step: function(state, circle) {
            circle.path.setAttribute('stroke', state.color);
            let value = Math.round(circle.value() * 60);
            circle.setText(value);
        }
        });

        circleA.animate(1.0);

        let containerB = document.getElementById("circleB");
        let circleB = new ProgressBar.Circle(containerB, {
        color: "#64DAF9",
        strokeWidth: 8,
        duration: 1600,
        from: { color: '#aaa' },
        to: { color: '#65daf9' },

        step: function(state, circle) {
            circle.path.setAttribute('stroke', state.color);
            let value = Math.round(circle.value() * 245);
            circle.setText(value);
        }
        });

        circleB.animate(1.0);

        let containerC = document.getElementById("circleC");
        let circleC = new ProgressBar.Circle(containerC, {
        color: "#64DAF9",
        strokeWidth: 8,
        duration: 2000,
        from: { color: '#aaa' },
        to: { color: '#65daf9' },

        step: function(state, circle) {
            circle.path.setAttribute('stroke', state.color);
            let value = Math.round(circle.value() * 32);
            circle.setText(value);
        }
        });

        circleC.animate(1.0);

        let containerD = document.getElementById("circleD");
        let circleD= new ProgressBar.Circle(containerD, {
        color: "#64DAF9",
        strokeWidth: 8,
        duration: 2200,
        from: { color: '#aaa' },
        to: { color: '#65daf9' },

        step: function(state, circle) {
            circle.path.setAttribute('stroke', state.color);
            let value = Math.round(circle.value() * 5243);
            circle.setText(value);
        }
        });

        circleD.animate(1.0);
    }
  },

  mounted() {
    this.circulos();
  }
}
</script>
