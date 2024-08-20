<script setup>
</script>

<template>
    <section>
        <h3>Mes projets</h3>
        <div class="content-container">
            <div class="projet">
                <img src="https://via.placeholder.com/400" alt="projet1">
                <span>
                    <h4>Projet 1</h4>
                    <button>En savoir plus</button>
                </span>
            </div>
            <div class="projet">
                <img src="https://via.placeholder.com/400" alt="projet2">
                <span>
                    <h4>Projet 2</h4>
                    <button>En savoir plus</button>
                </span>
            </div>
            <div class="projet">
                <img src="https://via.placeholder.com/400" alt="projet3">
                <span>
                    <h4>Projet 3</h4>
                    <button>En savoir plus</button>
                </span>
            </div>
        </div>
    </section>
</template>

<style scoped>
* {
    box-sizing: border-box;
}

section {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
}

h3 {
    display: flex;
    justify-content: center;
    width: 100%;
    font-size: x-large;
}

.content-container {
    display: flex;
    justify-content: space-around;
    width: 100%;
    flex-wrap: wrap;
}

.projet {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 1rem;
    padding: 1rem;
    border-radius: 10px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}

span {
    width: 100%;
    margin: 1rem;
    text-align: center;
}

button {
    padding: 10px 20px;
    font-weight: 500;
    background-color: #333;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

img {
    width: 100%;
    height: auto;
    border-radius: 10px;
}

@media (max-width: 460px) {
    .projet {
        width: 90%;
    }
}
</style>
