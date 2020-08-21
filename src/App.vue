<template>
  <div id="app">
    <img style="max-width:300px" alt="Vue logo" src="./assets/logo.png" />
    <SlotForm>
      <template v-slot:header>
        <h1>Form Title</h1>
      </template>
      <template v-slot:userName>
        <div class="form-group">
          <label for="exampleInputEmail1">Email address</label>
          <input
            type="email"
            class="form-control"
            id="exampleInputEmail1"
            aria-describedby="emailHelp"
          />
          <small
            id="emailHelp"
            class="form-text text-muted"
          >We'll never share your email with anyone else.</small>
        </div>
      </template>
    </SlotForm>
  </div>
</template>

<script>
import SlotForm from "./components/SlotForm.vue";

export default {
  name: "App",
  components: {
    SlotForm,
  },
};
</script>

<style>
#app {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
