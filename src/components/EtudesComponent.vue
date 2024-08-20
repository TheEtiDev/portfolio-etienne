<script setup>
</script>

<template>
    <section>
        <h3>Mes Études</h3>
        <div class="content-container">
            <div class="etude">
                <span class="entete">
                    <h4>Nom du programme 1</h4>
                    <h4>Nom de l'école 1</h4>
                    <img src="https://via.placeholder.com/100" alt="ecole1">
                </span>
                <span>
                    <p>Date de début - Date de fin</p>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit corporis voluptatum ipsa expedita
                        libero temporibus voluptatem dolores quos similique commodi. Harum ex consectetur impedit soluta
                        deserunt placeat voluptates? A, suscipit! Lorem ipsum dolor sit, amet consectetur adipisicing
                        elit. Illum omnis quos iste voluptatum molestias unde optio. Dolores mollitia asperiores eum
                        dignissimos, molestias cumque ex laborum commodi quis fugit repudiandae iste?</p>
                </span>
            </div>
            <div class="etude">
                <span class="entete">
                    <h4>Nom du programme 2</h4>
                    <h4>Nom de l'école 2</h4>
                    <img src="https://via.placeholder.com/100" alt="ecole2">
                </span>
                <span>
                    <p>Date de début - Date de fin</p>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Fugit corporis voluptatum ipsa expedita
                        libero temporibus voluptatem dolores quos similique commodi. Harum ex consectetur impedit soluta
                        deserunt placeat voluptates? A, suscipit! Lorem ipsum dolor sit, amet consectetur adipisicing
                        elit. Illum omnis quos iste voluptatum molestias unde optio. Dolores mollitia asperiores eum
                        dignissimos, molestias cumque ex laborum commodi quis fugit repudiandae iste?</p>
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

.etude {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 1rem;
    padding: 1rem;
    border: 1px solid #ccc;
    border-radius: 5px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}

img {
    width: 7.5rem;
    height: auto;
    margin: 1rem;
    border-radius: 50%;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}

h4 {
    font-size: 1rem;
    margin-bottom: 1rem;
    display: flex;
    justify-content: center;
}

span.entete {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    margin: 1rem 1rem 0 1rem;
    flex-wrap: wrap;
}

span {
    width: 100%;
    margin: 0 1rem 1rem 1rem;
    text-align: justify;
    padding: 0 1rem 0 1rem;
}
</style>
