<script setup>
</script>

<template>
    <section>
        <h3>Me contacter</h3>
        <div class="content-container">
            <div class="contact">
                <h4>Numéro de téléphone</h4>
                <p>123-456-9494</p>
                <button>Appeler</button>
            </div>
            <div class="contact">
                <h4>Courriel</h4>
                <p>test@test.com</p>
                <button>Copier le courriel</button>
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
    margin-bottom: 2rem;
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

.contact {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 1rem;
    padding: 1rem;
    border: 1px solid #ccc;
    border-radius: 5px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
    width: 30%;
    height: auto;
}

h4 {
    font-size: 1rem;
    margin-bottom: 1rem;
    display: flex;
    justify-content: center;
}

p {
    font-size: 1rem;
    margin-bottom: 1rem;
    display: flex;
    justify-content: center;
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

button:hover {
    background-color: #555;
}

@media (max-width: 660px) {
    .contact {
        width: 80%;
    }
}

</style>
