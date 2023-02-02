<template>
  <div>
    <h1>Sveiks!</h1>
    <h2>Izkatās, ka tu atrodies vecajā mājaslapā.</h2>
    <a href="">Spied šeit lai aizietu uz jauno!</a>
  </div>
</template>

<script setup>
  import { onMounted } from 'vue';

  onMounted(() => {
    document.title = "Vecrigas ekskursija | Vecā lapa"
  })
</script>

<style lang="scss">
  body, html {
    margin: 0;
    height: 100%;
  }

  body {
    position: relative;
    background-color: #171717;
    color: white;
    font-family: 'Roboto', sans-serif;

    text-align: center;
  }

  h1 {
    margin: 10pt;
    font-weight: 300;
    font-size: 30pt;
  }

  h2 {
    margin: 20pt;
    margin-bottom: 50pt;
    font-weight: 200;
    font-style: italic;
    font-size: 20pt;
  }

  a {
    text-decoration: none;
    color: white;
    text-align: center;

    font-family: 'Roboto', sans-serif;
    font-weight: 300;

    background-color: #202020;
    padding: 2%;
    margin: 10pt 0;

    border: 5pt solid #303030;
    border-radius: 20pt;

    transition: all 0.6s;
  }

  a:hover {
    background-color: #2c2c2c;
    border-color: #202020;

    transition: all 0.6s;
  }

  div {
    margin: 0;
    position: absolute;
    top: 50%;
    left: 50%;
    -ms-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);

    width: 100%;
  }
</style>
