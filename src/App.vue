<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <h1>Conversor Vue Js</h1>
    <div class="linha">
      <Conversor moeda-a="BRL" moeda-b="USD"/>
      <Conversor moeda-a='USD' moeda-b="BRL"/>
    </div>

    <div class="linha">
      <Conversor moeda-a="CAD" moeda-b="BRL"/>
      <Conversor moeda-a='BRL' moeda-b="CAD"/>
    </div>

    <div class="linha">
      <Conversor moeda-a="EURO" moeda-b="BRL"/>
      <Conversor moeda-a='BRL' moeda-b="EURO"/>
    </div>
    
  </div>
</template>

<script>

import Conversor from './components/Conversor';


export default {
  name: 'app',
  components: {
    Conversor
  }
}
</script>

<style>
#app {
  margin:auto;
  max-width: 900px;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.linha{
  margin-top: 40px;
  display: flex;
  justify-content: space-around;
}
</style>
