<template>
    <nav>
        <h2>
            <router-link to="/">Étienne Lessard</router-link>
        </h2>
        <ul>
            <li>
                <router-link to="/a-propos">À Propos</router-link>
            </li>
            <li>
                <router-link to="/projets">Projets</router-link>
            </li>
            <li>
                <router-link to="/experience">Expériences</router-link>
            </li>
            <li>
                <router-link to="/etudes">Études</router-link>
            </li>
            <li>
                <router-link to="/technologies">Technologies</router-link>
            </li>
            <li>
                <router-link to="/contact">Me Contacter</router-link>
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


    @media screen and (max-width: 975px) {
        ul {
            display: none;
        }

        nav {
            justify-content: center;
        }
    }
</style>