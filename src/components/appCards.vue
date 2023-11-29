<script>

export default {
    name: "appCards",

    props: [
        "cardList" // cardList coming from App
    ],

}

</script>


<template>
    <div class="all_cards_bg">
        <div class="all_cards_wrapper">

            <div class="all_cards">
                <div v-for="card in cardList" class="card">
                    <img :src=card.thumb alt="card image">
                    <p>{{ card.series }}</p>
                </div>
            </div>
            <div class="centered_button">
                <button class="card_btn">Load More</button>
            </div>
        </div>

    </div>
</template>


<style>
.all_cards_bg {
    background-color: black;
    height: 34rem;
}

.all_cards_wrapper {
    width: 70%;
    margin: 0 auto;
}

.all_cards {
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
    color: white;
    padding: 2rem 0;
}

.card {
    width: 10rem;
    height: 11rem;
    margin-bottom: 1rem;
}

.card img {
    width: 100%;
    height: 100%;
}

.card p {
    font-size: 0.80rem;
}

.centered_button {
    width: 7rem;
    margin: 2rem auto;


}

.card_btn {
    width: 7rem;
    height: 1.5rem;
    background-color: #3682f3;
    color: white;
    font-weight: bold;
    border-color: #3682f3;

}
</style>