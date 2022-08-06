
<template>
  <div class="app">
    <Sidebar />
    <router-view />
  </div>

</template>

<script setup>
  import Sidebar from './components/sidebar.vue'


</script>

<style lang="scss">
:root {
  --primary: #4ade80;
  --grey: #64748b;
  --dark: #334155;
  --light: #f1f5f9
  --sidebar-width: 300px;

}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Fira sans', sans-serif;
}

body {
      background: #4158D0;
    background: linear-gradient(
    115deg,
    rgba(86, 216, 228, 1) 10% ,
    rgba(159, 1, 234, 1) 90%);
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}

button {
  cursor: pointer;
  appearance: none;
  border: none;
  outline: none;
  background: none;
}

.app {
  display: flex;
  
  main {
    flex: 1 1 0;
    padding: 2rem;

    @media (max-width: 768px) {
      padding-left: 6rem;
    }
  }
}

</style>
