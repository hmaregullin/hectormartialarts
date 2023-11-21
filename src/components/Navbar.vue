<template>
  <div id="container">
    <nav id="navbar">
      <div class="header">
        <h2 class="channel">Hector Martial Arts</h2>
      </div>
      <div class="nav-links">
        <a href="#" class="nav-link">Home</a>
        <a href="#" class="nav-link">About</a>
        <a href="/#" class="nav-link">Contact</a>
      </div>
    </nav>
  </div>
</template>

<script lang="ts">
export default {
  data() {
    console.log('Hola');
  }
}
</script>

<style>
/* Font style */
@import url('https://fonts.googleapis.com/css2?family=Didact+Gothic&family=Roboto:wght@400;500;700&display=swap');

body {
  color: white;
  font-family: 'Didact Gothic', sans-serif; 
}

#navbar {
  background-color: rgb(30,30,30);
  display: flex;
  justify-content: space-between; /* Alinea los elementos al inicio y al final del navbar */
}

.header {
  display: flex;
  align-items: flex-start; /* Alinea el texto del encabezado hacia arriba */
}

.channel {
  margin-right: 15px; /* Añade un pequeño espacio entre el texto y los enlaces */
  margin-left: 15px;
}

.nav-links {
  display:block;
}

.nav-link {
  color: white;
  margin-right: 15px;
  margin-left: 15px;
  text-decoration: none;
}

.nav-link:hover {
  background-color: aliceblue;
  color: black;
}
</style>
