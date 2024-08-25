<script setup>
import { onMounted, ref } from 'vue';
// Import les images
import eventlitAnalyseDonnees from '@/assets/images/eventlit/eventlitAnalyseDonnees.png';
import eventlitCreerEvenement from '@/assets/images/eventlit/eventlitCreerEvenement.png';
import eventlitGererEvenement from '@/assets/images/eventlit/eventlitGererEvenement.png';
import eventlitInscription from '@/assets/images/eventlit/eventlitInscription.png';
import eventlitHome from '@/assets/images/eventlit/eventlitHome.png';

const eventlitImages = [
    eventlitAnalyseDonnees,
    eventlitAnalyseDonnees,
    eventlitCreerEvenement,
    eventlitGererEvenement,
    eventlitInscription,
    eventlitHome,
];

let eventlitImage = ref(null);

// Loader les images quand le composant est monté
onMounted(() => {
    eventlitImage.value = document.getElementById('eventlitImg');
});

// Logique pour changer les images
let currentImageIndex = 0;

setInterval(() => {
    currentImageIndex = (currentImageIndex + 1) % eventlitImages.length;
    eventlitImage.value.src = eventlitImages[currentImageIndex];
}, 4000);
</script>

<template>
    <section>
        <h3>Mes projets</h3>
        <div class="content-container">
            <div class="projet">
                <img id="eventlitImg" :src="eventlitHome" alt="eventlitImage">
                <span>
                    <h4>Eventlit</h4>
                    <router-link to="/eventlit" class="button-link">En savoir plus</router-link>
                </span>
            </div>
            <!-- <div class="projet">
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
            </div> -->
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
    width: 30%;
}

span {
    width: 100%;
    margin: 1rem;
    text-align: center;
}

.button-link {
    padding: 10px 20px;
    font-weight: 500;
    background-color: #333;
    color: white;
    border: none;
    text-decoration: none;
    border-radius: 5px;
    cursor: pointer;
}

.button-link:hover {
    background-color: #555;
}

img {
    width: 100%;
    height: 17rem;
    object-fit: cover;
    border-radius: 10px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}

@media (max-width: 1200px) {
    .projet {
        width: 45%;
    }
}

@media (max-width: 900px) {
    .projet {
        width: 60%;
    }
}

@media (max-width: 700px) {
    .projet {
        width: 90%;
    }
}
</style>
