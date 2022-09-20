<template>
  <main class='main'>
    <FormularioPrincipal :addData='addData' />
    <TablaPrincipal :data='data' />
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
  },
  data() {
    return {
      data: []
    }
  },
  methods: {
    addData(form) {
      this.data.push(form)
    }
  }
}
</script>
<!----------------------------------------------------------------------------------------------------------------->
<style>
body {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.app{
  margin: 0;
  padding: 0;
}
.main {
  padding: 5%;
  width: 90%;
  height: 90vh;
  background: linear-gradient(to bottom right, #3739b8, rgb(134, 151, 227));
  margin: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  gap: 3rem;
}
</style>