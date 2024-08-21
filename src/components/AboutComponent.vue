<script setup>
</script>

<template>
    <section>
        <h3>À propos de moi</h3>
        <div class="content-container">
            <img src="../assets/images/profilImg.jpg" alt="photo">
            <span>Je suis un passionné de technologie et d'apprentissage, toujours à la recherche de nouvelles
                connaissances et de défis à relever. Mes forces principales résident dans ma capacité exceptionnelle à
                apprendre par moi-même, ce qui me permet d'acquérir rapidement de nouvelles compétences et de m'adapter
                à des environnements changeants. Mon assiduité et mon sens des responsabilités font de moi un
                professionnel fiable et dévoué, tandis que mon leadership naturel me permet de guider et d'inspirer ceux
                qui m'entourent. Ces qualités combinées font de moi un atout précieux dans tout projet ou équipe
                auxquels je participe. </span>
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
}

img {
    width: 25%;
    height: auto;
    margin: 1rem;
    border-radius: 50%;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}

span {
    width: 50%;
    margin: 1rem;
    text-align: justify;
    line-height: 1.5rem;
    align-items: center;
    display: flex;
}

@media (max-width: 920px) {
    .content-container {
        flex-wrap: wrap;
        justify-content: center;
    }

    img {
        width: 30%;
    }

    span {
        width: 85%;
    }
}

@media (max-width: 600px) {

    img {
        width: 50%;
    }

    span {
        width: 85%;
    }
}
</style>
