<template>
  <form class="form">
    <h2 class="form__title">Formulario</h2>
    <div class="form__group">
      <label class="form__label" for="user">Usuario:</label>
      <input class="form__input" type="text" id="user" placeholder="Usuario">
    </div>
    <div class="form__group">
      <label class="form__label" for="course">Curso:</label>
      <div class='form__options'>
        <div>
          <input type="radio" id="react" name="course" value="react">
          <label class='form__help' for="react">React</label><br>
        </div>
        <div>
          <input type="radio" id="vue" name="course" value="vue">
          <label class='form__help' for="vue">Vue</label><br>
        </div>
        <div>
          <input type="radio" id="angular" name="course" value="angular">
          <label class='form__help' for="angular">Angular</label>
        </div>
      </div>
    </div>
    <div class="form__group">
      <label class="form__label" for="color">Colores:</label>
      <div class='form__options'>
        <div>
          <input type="checkbox" id="red" name="color" value="red">
          <label class='form__help' for="red">Rojo</label>
        </div>
        <div>
          <input type="checkbox" id="green" name="color" value="green">
          <label class='form__help' for="green">Verde</label>
        </div>
        <div>
          <input type="checkbox" id="blue" name="color" value="blue">
          <label class='form__help' for="blue">Azul</label>
        </div>
      </div>
    </div>
    <div class="form__group">
      <label class="form__label" for="bot">3 + 4 =</label>
      <input class="form__input" type="number" id="bot">
    </div>
    <div class='form__buttonContainer'>
      <button class='form__button'>Enviar</button>
    </div>
  </form>
</template>
<!----------------------------------------------------------------------------------------------------------------->
<script>
export default {
  name: 'FormularioPrincipal',
  props: {

  }
}
</script>
<!----------------------------------------------------------------------------------------------------------------->
<style scoped>
.form {
  background: #fff;
  border: 1px solid #a1a1a1;
  padding: 1rem;
  border-radius: 5px;
  width: 250px;
}

.form__title {
  font-size: 1.5rem;
  margin-bottom: 2rem;
  text-align: center;
  font-weight: 400;
}

.form__group {
  margin-bottom: 1.5rem;
  display: flex;
  flex-direction: column;
}

.form__options {
  display: flex;
  gap: 1rem;
  justify-content: center;
}

.form__label {
  font-size: 1.2rem;
  font-weight: 300;
  margin-bottom: .5rem;
}

.form__input {
  font-size: .8rem;
  font-weight: 300;
  border: 1px solid #707070;
  border-radius: 5px;
  padding: 5px;
}

.form__help {
  font-size: 1rem;
}

.form__buttonContainer {
  margin-top: 1rem;
  display: flex;
  justify-content: center;
}

.form__button {
  margin-top: 1rem;
  font-size: 1rem;
  background: #3739b8;
  color: #fff;
  padding: 5px 25px;
  border-radius: 5px;
  border: 1px solid #2a2ca8;
  transition: all 1s;
  cursor: pointer;
}

.form__button:hover {
  transform: scale(1.05);
}
</style>