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
</style>
