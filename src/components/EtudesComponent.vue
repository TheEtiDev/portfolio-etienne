<script setup>
</script>

<template>
    <section>
        <h3>Mes Études</h3>
        <div class="content-container">
            <div class="etude">
                <span class="entete">
                    <div>
                        <h4>Baccalauréat en génie logiciel</h4>
                        <h5>École de technologie supérieure (ÉTS)</h5>
                    </div>
                    <img src="../assets/images/LogoEts.jpg" alt="ecole1">
                </span>
                <span>
                    <p>avr. 2024 - août 2028 (prévue)</p>
                    <p>Je poursuis actuellement un Baccalauréat en génie logiciel à l'École de technologie supérieure
                        (ÉTS). Ce programme rigoureux me permet de développer une solide expertise en conception,
                        développement et gestion de logiciels. J'y apprends les principes fondamentaux de la
                        programmation, l'architecture logicielle, ainsi que la gestion de projets complexes. Les cours
                        couvrent également des domaines tels que les bases de données, les systèmes embarqués, et la
                        sécurité informatique. Grâce à une approche pratique axée sur les projets, j'acquiers non
                        seulement des compétences techniques, mais aussi une expérience concrète qui me prépare à
                        relever les défis du monde professionnel.</p>
                </span>
            </div>
            <div class="etude">
                <span class="entete">
                    <div>
                        <h4>Techniques en gestion et comptabilité</h4>
                        <h5>Cégep de Saint-Jérôme</h5>
                    </div>
                    <img src="../assets/images/LogoCstj.jpg" alt="ecole2">
                </span>
                <span>
                    <p>août	2021 - avr. 2024</p>
                    <p>J'ai complété un programme en Techniques de gestion et comptabilité au Cégep de Saint-Jérôme, où
                        j'ai acquis une compréhension approfondie des aspects critiques de la gestion d'entreprise et
                        des affaires. Ce programme m'a permis de me familiariser avec des domaines clés tels que le
                        marketing, les ressources humaines, et l'approvisionnement, tout en développant une expertise
                        approfondie en comptabilité et gestion financière. De plus, j'ai pu renforcer mes compétences en
                        gestion de projets, ce qui m'a préparé à gérer efficacement les opérations et les finances au
                        sein d'une entreprise.</p>
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

p {
    line-height: 1.5;
}
</style>
