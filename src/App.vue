<script>
import appHeader from './components/appHeader.vue';
import appFooter from './components/appFooter.vue';
import appCards from './components/appCards.vue';

export default {


  components: {
    appHeader,
    appFooter,
    appCards,
  },

  data() {
    return {

      cards: // Array for cards which are proped in appCards
        [
          {
            thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
            price: "$19.99",
            series: "Action Comics",
            type: "comic book",
          },
          {
            thumb: "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
            price: "$3.99",
            series: "American Vampire 1976",
            type: "comic book",
          },
          {
            thumb: "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
            price: "$16.99",
            series: "Aquaman",
            type: "graphic novel",
          },
          {
            thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
            price: "$2.99",
            series: "Batgirl",
            type: "comic book",
          },
          {
            thumb: "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
            price: "$3.99",
            series: "Batman",
            type: "comic book",
          },
          {
            thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
            price: "$2.99",
            series: "Batman Beyond",
            type: "comic book",
          },
          {
            thumb: "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
            price: "$3.99",
            series: "Batman/Superman",
            type: "comic book",
          },
          {
            thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
            price: "$4.99",
            series: "Batman/Superman Annual",
            type: "comic book",
          },
          {
            thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
            price: "$5.99",
            series: "Batman: The Joker War Zone",
            type: "comic book",
          },
          {
            thumb: "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
            price: "$6.99",
            series: "Batman: Three Jokers",
            type: "comic book",
          },
          {
            thumb: "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
            price: "$4.99",
            series: "Batman: White Knight Presents: Harley Quinn",
            type: "comic book",
          },
          {
            thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
            price: "$16.99",
            series: "Catwoman",
            type: "graphic novel",
          },
        ]
    }
  }
}

</script>

<!-- HTML Section -->
<template>
  <!-- Header Section -->
  <appHeader />

  <!-- Juumbtron Section -->

  <div class="jumbotron">
    <img class="jumbo" src="/img/jumbotron.jpg" alt="">
  </div>
  <div class="badge">
    <span>CURRENT SERIES</span>
  </div>

  <!-- Cards Section -->
  <div class="all_cards_bg">
    <div class="all_cards_wrapper">
      <div class="all_cards">
        <appCards v-for="card in cards" :image="card.thumb" :title="card.series" />
      </div>
      <div class="centered_button">
        <button class="card_btn">LOAD MORE</button>
      </div>
    </div>
  </div>

  <!-- Footer Section -->
  <appFooter />
</template>

<!-- Styling Section -->
<style scoped>
.wrapper {
  width: 75%;
  margin: 0 auto;
}

.jumbotron {
  width: 100%;
  height: 25rem;
  overflow: hidden;
  position: relative;
}

.jumbo {
  width: 100%;
}

.badge {
  color: white;
  width: 10rem;
  height: 2rem;
  background-color: #3682f3;
  text-align: center;
  padding: 0.5rem;
  font-weight: bold;
  position: absolute;
  top: 30rem;
  left: 14rem;
}

.centered_button {
  width: 7rem;
  margin: 2rem auto;
}

.card_btn {
  width: 9rem;
  height: 2rem;
  background-color: #3682f3;
  color: white;
  font-weight: bold;
  border-color: #3682f3;

}

.all_cards_bg {
  background-color: black;
  height: 36rem;
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
</style>
