<template>
    <nav>
        <h2>Étienne Lessard</h2>
        <ul>
            <li>
                <router-link to="/">Home</router-link>
            </li>
            <li>
                <router-link to="/about">About</router-link>
            </li>
            <li>
                <router-link to="/projects">Projects</router-link>
            </li>
            <li>
                <router-link to="/contact">Contact</router-link>
            </li>
            <li>
                <router-link to="/blog">Blog</router-link>
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
    }


    @media screen and (max-width: 600px) {
        ul {
            display: none;
        }

        nav {
            justify-content: center;
        }
    }
</style>