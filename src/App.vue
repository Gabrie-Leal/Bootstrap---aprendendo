<template>
  <div>
    <HeaderNavegacao/>
    <ConteudoMain/>
  </div>
</template>

<script>
import HeaderNavegacao from "./components/HeaderNavegacao.vue"
import ConteudoMain from "./components/ConteudoMain.vue"

export default {
  components: {
    HeaderNavegacao,
    ConteudoMain,
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

.about-title{
    font-size: 17px;
    color:#444;
    text-transform: uppercase;
    font-weight: bold;
}
</style>
