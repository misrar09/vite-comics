<script>

export default {
    name: "appCards",

    props: [
        "image", "title" // coming from App
    ],

}
</script>

<template>
    <div class="card">
        <img :src=image alt="card image">
        <p>{{ title.toUpperCase() }}</p>
    </div>
</template>


<style>
.card {
    width: 10rem;
    height: 11rem;
    margin-bottom: 2rem;
}

.card img {
    width: 100%;
    height: 100%;
}

.card p {
    font-size: 0.80rem;
    padding-top: 0.5rem;
}
</style>