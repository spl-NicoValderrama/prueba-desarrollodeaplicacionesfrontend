<template>
  <div class="home">
    <h1>Pruebas</h1>
    <hr />
    <section>
      <h2 class="titles">Ejercicio 1</h2>
      <ContadorComponent />
    </section>
    <hr />
    <section>
      <h2 class="titles">Ejercicio 2</h2>
      <div class="exercise-2">
        <h3 for="">Rutas del "Router"</h3>
        <nav>
          <router-link to="/">Home</router-link> |
          <router-link to="/about">About</router-link> |
          <router-link to="/contact">Contact</router-link>
        </nav>
      </div>
    </section>
    <hr />
    <section>
      <h2 class="titles">Ejercicio 3</h2>
      <ParentComponent />
    </section>
    <br />
    <hr />
  </div>
</template>

<script>
import ContadorComponent from "@/components/ContadorComponent.vue";
import ParentComponent from "@/components/ParentComponent.vue";

export default {
  name: "HomeView",
  components: {
    ContadorComponent,
    ParentComponent,
  },
};
</script>

<style>
.titles {
  margin-left: 4rem;
  text-align: left;
  padding-top: 1.5%;
}

.exercise-2 {
  padding-top: 2%;
  padding-bottom: 2%;
}

h1 {
  margin-bottom: 3%;
}
</style>
