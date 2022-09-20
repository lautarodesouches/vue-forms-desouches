<template>
  <main class='main'>
    <FormularioPrincipal />
    <TablaPrincipal />
  </main>
</template>
<!----------------------------------------------------------------------------------------------------------------->
<script>
import FormularioPrincipal from './components/FormularioPrincipal.vue';
import TablaPrincipal from './components/TablaPrincipal.vue';

export default {
  name: 'App',
  components: {
    FormularioPrincipal,
    TablaPrincipal
  }
}
</script>
<!----------------------------------------------------------------------------------------------------------------->
<style>
body {
  margin: 0;
}

.main {
  width: 100vw;
  height: 100vh;
  background: linear-gradient(to bottom right, #3739b8, rgb(134, 151, 227));
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>