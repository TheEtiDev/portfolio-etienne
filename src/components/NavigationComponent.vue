<template>
    <nav>
        <h2>
            <a href="/#home">Étienne Lessard</a>
        </h2>
        <ul>
            <li>
                <a href="/#a-propos">À Propos</a>
            </li>
            <li>
                <a href="/#projets">Projets</a>
            </li>
            <li>
                <a href="/#experiences">Expériences</a>
            </li>
            <li>
                <a href="/#etudes">Études</a>
            </li>
            <li>
                <a href="/#contact">Me Contacter</a>
            </li>
        </ul>
    </nav>
</template>

<script setup>

</script>

<style scoped>
nav {
    background-color: #333;
    color: white;
    width: 100%;
    display: flex;
    align-items: center;
}

h2 {
    margin: 1rem;
}

ul {
    display: flex;
    justify-content: right;
    list-style: none;
    padding: 0;
    flex-grow: 1;
    font-weight: 700;
}

li {
    margin: 0 1rem;
}

a {
    color: white;
    text-decoration: none;
}

a:hover {
    text-decoration: underline;
    color: #ccc;
}

html {
    scroll-behavior: smooth;
}


@media screen and (max-width: 975px) {
    ul {
        display: none;
    }

    nav {
        justify-content: center;
    }
}
</style>