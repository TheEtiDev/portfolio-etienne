<script setup>
</script>

<template>
    <section>
        <h3>À propos de moi</h3>
        <div class="content-container">
            <img src="https://via.placeholder.com/1080x1080" alt="photo">
            <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. In sunt assumenda dolor atque optio tenetur
                veniam eveniet magni, distinctio qui minus esse expedita facilis hic totam necessitatibus reprehenderit,
                non voluptate! Lorem ipsum dolor sit amet consectetur adipisicing elit. In sunt assumenda dolor atque
                optio tenetur veniam eveniet magni, distinctio qui minus esse expedita facilis hic totam necessitatibus
                reprehenderit, non voluptate! <br> Lorem ipsum dolor sit amet consectetur adipisicing elit. In sunt
                assumenda dolor atque optio tenetur veniam eveniet magni, distinctio qui minus esse expedita facilis hic
                totam necessitatibus reprehenderit, non voluptate! Lorem ipsum dolor sit amet consectetur adipisicing
                elit. In sunt assumenda dolor atque optio tenetur veniam eveniet magni, distinctio qui minus esse
                expedita facilis hic totam necessitatibus reprehenderit, non voluptate! </span>
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
