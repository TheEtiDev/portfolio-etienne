<script setup>
import NavigationComponent from '../components/NavigationComponent.vue';
import FooterComponent from '../components/FooterComponent.vue';
</script>

<template>
    <NavigationComponent />
    <section>
        <h2>Eventlit</h2>
        <div class="table-matiere-conteneur">
            <h3>Table des matières</h3>
            <ul class="table-matieres">
                <li><a href="#eventlit-description">Brève description</a></li>
                <li><a href="#eventlit-technologies">Technologies utilisées</a></li>
                <li><a href="#eventlit-contexte">Contexte et but</a></li>
                <li><a href="#eventlit-architecture">Architecture</a></li>
                <li><a href="#eventlit-interface-web">Interface web</a></li>
                <li><a href="#eventlit-interface-mobile">Interface mobile</a></li>
                <li><a href="#eventlit-apprentissages">Ce que j'ai appris</a></li>
            </ul>
        </div>
        <dev class="tech-description-conteneur">
            <div class="description-conteneur">
                <h3 id="eventlit-description">Brève description</h3>
                <p>Eventlit est une application full stack conçue pour créer et gérer des événements avec lesquels les
                    utilisateurs peuvent interagir. Cette solution se compose d'une interface web destinée aux organisateurs
                    d'événements, ainsi que d'une application mobile native pour Android, dédiée aux utilisateurs. Les deux
                    interfaces communiquent via une API REST commune, assurant une expérience cohérente et harmonieuse.</p>
            </div>
            <div class="technologies-conteneur">
                <h3 id="eventlit-technologies">Technologies utilisées</h3>
                <ul>
                    <li>Android Studio</li>
                    <li>CSS</li>
                    <li>Composer</li>
                    <li>Docker</li>
                    <li>Git</li>
                    <li>GitHub</li>
                    <li>HTML</li>
                    <li>Jackson</li>
                    <li>Java</li>
                    <li>JavaScript</li>
                    <li>Laravel</li>
                    <li>MySQL</li>
                    <li>Ngrok</li>
                    <li>NodeJS</li>
                    <li>OkHttp</li>
                    <li>PHP</li>
                    <li>Vue.js</li>
                    <li>Vercel</li>
                    <li>Vite</li>
                </ul>
            </div>
        </dev>
        <div class="contexte-but-conteneur">
            <h3 id="eventlit-contexte">Contexte et but</h3>
            <p>Cette application a été conçue dans le cadre de mon cours universitaire de projet intégrateur et a été
                réalisée en équipe. J'ai pris en charge l'intégralité du développement backend, incluant la création de
                l'API et la gestion de la base de données, ainsi que la mise en place des requêtes HTTP pour les
                applications mobile et web. J'ai également contribué au design de l'interface web. L'objectif de notre
                application était de créer une plateforme permettant aux organisateurs d'événements de promouvoir leurs
                activités et d'offrir aux utilisateurs un moyen simple de découvrir et de participer aux événements qui
                les intéressent. </p>
        </div>
        <div class="architecture-conteneur">
            <h3 id="eventlit-architecture">Architecture</h3>
            <ul class="image-display">
                <li>
                    <img src="../assets/images/eventlit/eventlitArchitecture.png" alt="eventlitArchitecture" id="architectureImg">
                </li>
            </ul>
            <p>Eventlit se compose de deux interfaces distinctes, chacune répondant à des préoccupations spécifiques.
                L'interface web, conçue avec Vue.js, permet aux organisateurs de gérer l'ensemble des opérations liées à
                la création et à la gestion de leurs événements. L'interface mobile, développée avec Android Studio en
                Java, permet aux utilisateurs de consulter les événements, effectuer des recherches, s'inscrire, et bien
                plus encore. Pour garantir la cohérence des données entre les applications web et mobile, ces deux
                interfaces communiquent avec une API REST développée avec Laravel, qui interagit avec notre base de
                données MySQL pour fournir des réponses adaptées aux différentes requêtes. Afin de simplifier le
                déploiement de l'API sur différentes machines et de faciliter le développement, Docker a été utilisé
                pour permettre une installation aisée du backend sur les différentes infrastructures nécessaires à
                l'application.</p>
            <p>Pour la gestion de l'authentification des utilisateurs, nous avons adopté le principe du JSON Web Token
                (JWT), implémenté à l'aide de Laravel Sanctum. Cette approche nous permet de générer et d'envoyer un
                jeton personnalisé à chaque utilisateur après une connexion réussie à son compte. Ce jeton unique est
                ensuite utilisé pour authentifier les requêtes HTTP adressées à notre API, garantissant ainsi que seules
                les requêtes provenant d'utilisateurs authentifiés sont traitées. Grâce à cette méthode, nous renforçons
                la sécurité de notre application en protégeant les données des utilisateurs et en empêchant tout accès
                non autorisé. De plus, Laravel Sanctum offre une gestion simplifiée des sessions utilisateur, ce qui
                facilite la gestion des connexions multiples et améliore l'expérience utilisateur sur les interfaces web
                et mobile.</p>
            <p>Au cours du développement de l'application, j'ai mis en place un serveur qui nous a permis de déployer
                notre backend en ligne, accélérant ainsi le développement et les tests de nos interfaces front-end. Ce
                serveur a été configuré avec Ngrok, permettant d'exposer facilement notre backend via un endpoint HTTPS
                sécurisé.</p>
        </div>
        <div class="web-conteneur">
            <h3 id="eventlit-interface-web">Interface web</h3>
            <ul class="image-display">
                <li>
                    <img src="../assets/images/eventlit/eventlitHome.png" alt="eventlitHome">
                </li>
                <li>
                    <img src="../assets/images/eventlit/eventlitCreerEvenement.png" alt="eventlitCreerEvenement">
                </li>
                <li>
                    <img src="../assets/images/eventlit/eventlitGererEvenement.png" alt="eventlitGererEvenement">
                </li>
                <li>
                    <img src="../assets/images/eventlit/eventlitInscription.png" alt="eventlitInscription">
                </li>
                <li>
                    <img src="../assets/images/eventlit/eventlitAnalyseDonnees.png" alt="eventlitAnalyseDonnees">
                </li>
            </ul>
            <p>L'interface web est conçue pour gérer toutes les fonctionnalités liées à la création et à la gestion des
                événements. Plus précisément, elle permet aux utilisateurs de créer un compte et de se connecter à un
                compte existant, de créer des événements en fonction de critères requis et optionnels, et d'ajouter des
                étiquettes pour regrouper les événements selon différentes catégories. Les organisateurs peuvent
                également consulter les données de performance de leurs événements, telles que le nombre d'inscriptions
                ou le nombre d'impressions, et accéder aux messages de feedback laissés par les utilisateurs. Des
                fonctionnalités de modification et de suppression sont également disponibles, permettant aux
                organisateurs de maintenir un contrôle total sur leurs événements. Pour garantir une expérience
                utilisateur fluide et sécurisée, les éléments des formulaires sont validés côté client pour prévenir les
                erreurs, ainsi que côté serveur pour empêcher toute exploitation potentielle.</p>
        </div>
        <div class="mobile-conteneur">
            <h3 id="eventlit-interface-mobile">Interface mobile</h3>
            <ul class="image-display">
                <li>
                    <img src="../assets/images/eventlit/eventlitMobileHome.png" alt="eventlitMobileHome">
                </li>
                <li>
                    <img src="../assets/images/eventlit/eventlitMobileInscription.png" alt="eventlitMobileEvenement">
                </li>
                <li>
                    <img src="../assets/images/eventlit/eventlitMobileLogin.png" alt="eventlitMobileInscription">
                </li>
                <li>
                    <img src="../assets/images/eventlit/eventlitMobileRecherche.png" alt="eventlitMobileLogin">
                </li>
            </ul>
            <p>
                L'interface mobile est conçue pour offrir aux utilisateurs toutes les fonctionnalités nécessaires afin
                de pouvoir interagir pleinement avec les événements disponibles sur l'application. Elle permet notamment
                de gérer l'authentification des utilisateurs, de modifier les paramètres de l'application, de rechercher
                des événements par nom ou étiquette, de consulter les informations des événements, et de s'y inscrire.
                De plus, l'interface mobile permet aux utilisateurs d'envoyer des messages de feedback aux
                organisateurs. Tout comme l'interface web, l'interface mobile est conçue pour offrir une expérience
                utilisateur fluide et sécurisée, avec une validation des données des formulaires effectuée tant côté
                client que côté serveur. L'application mobile propose également des options de personnalisation,
                permettant aux utilisateurs de changer la langue de l'interface et de choisir entre un mode sombre et un
                mode clair.</p>
        </div>
        <div class="apprentissages-conteneur">
            <h3 id="eventlit-apprentissages">Ce que j'ai appris</h3>
            <p>Durant la conception et le développement de ce projet, j'ai eu l'opportunité d'apprendre et de mettre en
                pratique
                plusieurs concepts clés du génie logiciel. J'ai notamment pu développer cette application en suivant les
                principes de la méthodologie AGILE et du framework SCRUM, ce qui nous a permis de mener à bien le projet
                en deux
                sprints de deux semaines à temps partiel. Cette approche nous a non seulement aidés à structurer notre
                travail
                de manière efficace, mais elle a également renforcé notre capacité à collaborer et à nous adapter
                rapidement aux
                besoins changeants du projet.</p>
            <p>De plus, ce projet m'a permis d'acquérir une solide expérience avec le framework Laravel et d'approfondir
                mes
                connaissances en utilisant Docker pour le déploiement. Bien que je reconnaisse que plusieurs autres
                fonctionnalités pourraient être ajoutées pour rendre ce produit véritablement attractif pour les
                utilisateurs,
                les apprentissages et les compétences que j'ai développés au cours de ce projet en font une expérience
                extrêmement précieuse. Ce projet a non seulement enrichi mes connaissances techniques, mais il m'a
                également
                permis de renforcer mes compétences en gestion de projet et en développement logiciel.</p>
        </div>

        <a href="/" class="button-link">Retour à la page principale</a>
    </section>
    <FooterComponent />
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

h2 {
    display: flex;
    justify-content: center;
    width: 100%;
    font-size: x-large;
}

.table-matiere-conteneur {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 95%;
    border: none;
    box-shadow: none;
}

div {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin: 2rem 0 2rem 0;
    padding: 1rem;
    border: 1px solid #ccc;
    border-radius: 5px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}


h3 {
    display: flex;
    justify-content: center;
    width: 100%;
    font-size: large;
    align-items: center;
}

.table-matieres {
    display: flex;
    flex-direction: column;
    align-items: center;
    list-style-type: none;
    text-decoration: underline;
    padding: 1rem;
    width: 20rem;
    border-radius: 1rem;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}

.table-matieres li {
    margin: 0.5rem 0;
}

.table-matieres a {
    text-decoration: none;
    color: #333;
}

.table-matieres a:hover {
    color: #007bff;
}

p {
    width: 100%;
    margin: 1rem;
    text-align: justify;
    line-height: 1.5rem;
    padding: 0 1rem 0 1rem;
}

.tech-description-conteneur {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    width: 95%;
    margin-bottom: 1rem;
}

.description-conteneur, .technologies-conteneur{
    flex-basis: 45%;
    flex-grow: 1;
    box-sizing: border-box;
    margin-bottom: 1rem;
    margin: 1rem 2.5% 1rem 2.5%;
}

.contexte-but-conteneur {
    width: 90%;
}

.architecture-conteneur {
    width: 90%;
}

ul.image-display {
    list-style-type: none;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    padding: 0;
    margin: 0;
    width: 100%;
}

img {
    width: 100%;
    height: 20rem;
    object-fit: cover;
    border-radius: 10px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
}

#architectureImg {
    height: 35rem;
}

.architecture-conteneur img {
    width: 100%;
    max-width: 800px;
    margin: 1rem 0;
}

.web-conteneur {
    width: 90%;
}

.web-conteneur img {
    width: 100%;
    max-width: 800px;
    margin: 1rem 0;
}

.mobile-conteneur {
    width: 90%;
}

.mobile-conteneur img {
    width: 100%;
    max-width: 800px;
    margin: 1rem 0;
}

.apprentissages-conteneur {
    width: 90%;
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
    margin: 1rem;
}

.button-link:hover {
    background-color: #555;
}

@media (max-width: 765px) {
    img {
        height: auto;
    }

    #architectureImg {
        height: auto;
    }
}
</style>
