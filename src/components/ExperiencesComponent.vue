<script setup>
</script>

<template>
    <section>
        <h3>Mes expériences</h3>
        <div class="content-container">
            <div class="experience">
                <span class="entete">
                    <div>
                        <h4>Coordonnateur marketing numérique</h4>
                        <h5>Sept24</h5>
                    </div>
                    <img src="../assets/images/LogoSept24.jpg" alt="experience1">
                </span>
                <span>
                    <p>sept. 2021 - avr. 2024 - 2 ans 8 mois</p>
                    <p>En tant que coordonnateur marketing numérique chez Set24, j'ai eu l'opportunité de travailler sur
                        la création, l'optimisation, et la gestion de campagnes numériques. J'ai utilisé divers outils
                        publicitaires tels que Facebook Ads, Google Ads, LinkedIn Ads, TikTok Ads, Spotify Ads, et
                        Snapchat Ads. Dans le cadre de mon rôle, j'ai élaboré des stratégies marketing adaptées aux
                        besoins de mes clients et présenté les résultats des campagnes à ces derniers.</p>
                    <p>Ce poste à
                        distance m'a permis de développer les compétences nécessaires pour travailler efficacement sur
                        des projets d'agence. J'ai collaboré sur divers types de campagnes, notamment des campagnes
                        publicitaires sur les moteurs de recherche (SEM), des campagnes de génération de leads, et des
                        campagnes de notoriété sur les réseaux sociaux. Enfin, j'ai collaboré avec le département de
                        développement web pour intégrer des outils d'analytique et apporter des modifications aux sites
                        web des clients afin d'optimiser leurs efforts marketing.</p>
                </span>
            </div>
            <div class="experience">
                <span class="entete">
                    <div>
                        <h4>Caissier</h4>
                        <h5>Matériaux Pont-Masson</h5>
                    </div>
                    <img src="../assets/images/LogoPont-Masson.jpg" alt="experience2">
                </span>
                <span>
                    <p>mai 2020 - oct 2021 - 1 an 6 mois</p>
                    <p>En tant que caissier chez Matériaux Pont-Masson, j'ai assuré la gestion des transactions
                        quotidiennes, notamment les retours et les achats des clients.</p>
                    <p>
                        Mon efficacité et mon sens des
                        responsabilités m'ont permis d'être promu au rôle de caissier gestionnaire des dépôts des
                        caisses. Dans ce rôle, j'étais responsable de la gestion du coffre de liquidités de l'entreprise
                        et de la préparation des dépôts bancaires quotidiens, garantissant ainsi l'exactitude et la
                        sécurité des fonds.
                    </p>
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

.experience {
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
</style>
