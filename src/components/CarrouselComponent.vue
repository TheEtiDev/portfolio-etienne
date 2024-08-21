<script setup>
import { onMounted } from 'vue';

let slideIndex = 1;

onMounted(() => {
    showSlide(slideIndex);
});

function plusSlides(n) {
    showSlide(slideIndex += n);
}

function currentSlide(n) {
    //Présentement désactiver pour éviter les erreurs
    //showSlide(slideIndex = n);
}

function showSlide(n) {
    let i;
    let slides = document.getElementsByClassName("slide");
    let dots = document.getElementsByClassName("dot");


    if (n > slides.length) {
        slideIndex = 1;
    }

    if (n < 1) {
        slideIndex = slides.length;
    }

    for (i = 0; i < slides.length; i++) {
        slides[i].style.display = "none";
    }

    for (i = 0; i < dots.length; i++) {
        dots[i].className = dots[i].className.replace(" active", "");
    }

    slides[slideIndex - 1].style.display = "block";
    dots[slideIndex - 1].className += " active";
}

// Auto slide change
setInterval(() => {
    plusSlides(1);
}, 6000);
</script>

<template>
    <div class="carrousel-container">
        <div class="slide fade">
            <img src="../assets/images/experienceImg.jpg" alt="slide1">
            <div class="slide-content">
                <h2>Expériences</h2>
                <button>Voir plus de détails</button>
            </div>
        </div>
        <div class="slide fade">
            <img src="../assets/images/etudesImg.jpg" alt="slide2">
            <div class="slide-content">
                <h2>Études</h2>
                <button>Voir plus de détails</button>
            </div>
        </div>
        <div class="slide fade">
            <img src="../assets/images/technologiesImg.jpg" alt="slide3">
            <div class="slide-content">
                <h2>Technologies</h2>
                <button>Voir plus de détails</button>
            </div>
        </div>
        <div class="slide fade">
            <img src="../assets/images/projetsImg.jpg" alt="slide4">
            <div class="slide-content">
                <h2>Projets</h2>
                <button>Voir plus de détails</button>
            </div>
        </div>
        <div class="slide fade">
            <img src="../assets/images/contactImg.jpg" alt="slide5">
            <div class="slide-content">
                <h2>Me Contacter</h2>
                <button>Voir plus de détails</button>
            </div>
        </div>
    </div>

    <!-- Les points pour la navigation -->
    <div class="nav-dots">
        <span class="dot" @click="currentSlide(1)"></span>
        <span class="dot" @click="currentSlide(2)"></span>
        <span class="dot" @click="currentSlide(3)"></span>
        <span class="dot" @click="currentSlide(4)"></span>
        <span class="dot" @click="currentSlide(5)"></span>
    </div>

</template>


<style scoped>
.nav-dots {
    text-align: center;
}

img {
    width: 100%;
    height: auto;
    filter: brightness(85%);
}

* {
    box-sizing: border-box;
}

h2 {
    font-size: 3rem;
    margin-bottom: 1rem;
}

button {
    padding: 10px 20px;
    font-weight: 600;
    background-color: #333;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background-color: #555;
}

.carrousel-container {
    max-width: 100%;
    position: relative;
    margin: auto;
}

.slide {
    display: none;
}

.next,
.prev {
    cursor: pointer;
    position: absolute;
    top: 50%;
    width: auto;
    padding: 16px;
    margin-top: -22px;
    color: white;
    font-weight: bold;
    font-size: 18px;
    transition: 0.6s ease;
    border-radius: 0 3px 3px 0;
    user-select: none;
}

.next {
    right: 0;
    border-radius: 3px 0 0 3px;
}

.prev:hover,
.next:hover {
    background-color: rgba(0, 0, 0, 0.8);
}

.slide-content {
    position: absolute;
    justify-content: center;
    text-align: center;
    color: white;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

.nav-dots {
    transform: translate(0, -2rem);
}

.dot {
    /* cursor: pointer; */
    height: 15px;
    width: 15px;
    margin: 0 2px;
    background-color: #bbb;
    border-radius: 50%;
    display: inline-block;
    transition: background-color 0.6s ease;
}

/* .active,
.dot:hover {
    background-color: #717171;
} */

.active {
    background-color: #717171;
}

.fade {
    animation-name: fade;
    animation-duration: 1.5s;
}

@keyframes fade {
    from {
        opacity: .4
    }

    to {
        opacity: 1
    }
}

@media screen and (max-width: 610px) {
    h2 {
        font-size: 2rem;
    }
}

@media screen and (max-width: 405px) {
    h2 {
        font-size: 1.5rem;
    }
}
</style>