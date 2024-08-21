<script setup>
</script>

<template>
  <footer>
    <span>Par Étienne Lessard</span>
    <router-link to="/credits">Crédits</router-link>
    <span>Fait avec VueJS</span>
  </footer>
</template>

<style scoped>
    footer {
        background-color: #333;
        color: white;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 50px;
        display: flex;
        justify-content: space-around;
    }
    
    a {
        color: white;
    }
    
    a:hover {
        color: #ccc;
    }
</style>
