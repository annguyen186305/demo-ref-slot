<template>
  <div id="app">
    <demoRef/>
    <demoSlot class="app-slot"></demoSlot>
    <script type="module" src="https://unpkg.com/ionicons@7.1.0/dist/ionicons/ionicons.esm.js"></script>
  </div>
</template>

<script>
import demoRef from "@/components/demoRef.vue";
import DemoSlot from "@/components/demoSlot.vue";

export default {
  name: 'App',
  components: {
    DemoSlot,
    demoRef
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
