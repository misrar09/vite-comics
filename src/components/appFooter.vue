<script>
export default {
    name: "appFooter",
    data() {
        return {
            categories: [
                {
                    image: "./img/buy-comics-digital-comics.png",
                    text: "DIGITAL COMICS"
                },
                {
                    image: "./img/buy-comics-merchandise.png",
                    text: "DC MERCHANDISE"
                },
                {
                    image: "./img/buy-comics-subscriptions.png",
                    text: "SUBSCRITPTOIN",
                },
                {
                    image: "./img/buy-comics-shop-locator.png",
                    text: "COMIC SHOP LOCATOR",
                },
                {
                    image: "./img/buy-dc-power-visa.svg",
                    text: "DC POWER VISA",
                },
            ]
        }
    }
}

</script>

<template>
    <section class="categories">
        <div class="cat_wrapper">
            <div v-for="category in categories" class="cats ">
                <img :src="category.image" alt="image">
                <span>{{ category.text }}</span>
            </div>
        </div>
    </section>
    <section class="secondSection ">
        <div class="col_wrapper">
            <div>
                <div class="col">
                    <h4>DC COMICS</h4>
                    <a href="#">Characters</a>
                    <a href="#">Comics</a>
                    <a href="#">Movies</a>
                    <a href="#">TV</a>
                    <a href="#">Games</a>
                    <a href="#">Videos</a>
                    <a href="#">News</a>
                </div>
                <div class="col" l>
                    <h4>SHOP</h4>
                    <a href="#">Shop DC</a>
                    <a href="#">Shop DC Collectibles</a>
                </div>
            </div>
            <div class="col">
                <h4>DC</h4>
                <a href="#">Characters</a>
                <a href="#">Terms Of Use</a>
                <a href="#">Privacy policy (New)</a>
                <a href="#">Ad Choices</a>
                <a href="#">Adverstising</a>
                <a href="#">Jobs</a>
                <a href="#">Subscriptions</a>
                <a href="#">Talent Workshops</a>
                <a href="#">CPSC Certificates</a>
                <a href="#">Ratings</a>
                <a href="#">Shop Help</a>
                <a href="#">Contact Us</a>
            </div>
            <div class="col">
                <h4>SITES</h4>
                <a href="#">DC</a>
                <a href="#">MAD Magazine</a>
                <a href="#">DC Kids</a>
                <a href="#">DC Universe</a>
                <a href="#">DC Power Visa</a>
            </div>
            <div class="dc_bg">
                <!-- <img class="dc_bg" src="/img/dc-logo-bg.png" alt=""> -->
            </div>
        </div>
    </section>
    <section class="thirdSection">
        <div class="third_sec_wrapper">
            <div class="sing_up">
                <h5>SIGN-UP NOW!</h5>
            </div>
            <div class="follow_us">
                <div>
                    <h4>FOLLOW US</h4>
                </div>
                <div>
                    <i class="fa-brands fa-facebook"></i>
                    <i class="fa-brands fa-twitter"></i>
                    <i class="fa-brands fa-youtube"></i>
                    <i class="fa-brands fa-pinterest"></i>
                    <i class="fa-solid fa-location-dot"></i>
                </div>
            </div>
        </div>
    </section>
</template>



<style scoped>
.categories {
    background-color: #3682f3;
    height: 8rem;

}

.cat_wrapper {
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    width: 75%;
    margin: 0 auto;
}

.cats {
    display: flex;
    align-items: center;
    padding: 1.5rem;
    font-size: 0.85rem;
    color: white;
}

.cats span {
    padding: 1rem;
}

.cats img {
    width: 3rem;
}

.secondSection {
    background-image: url(./img/footer-bg.jpg);
    height: 24rem;
}

.col_wrapper {
    display: flex;
    width: 75%;
    margin: 0 auto;
}

.col {
    display: flex;
    flex-direction: column;
    padding: 2rem;
    color: white;
}

.dc_bg {
    width: 60%;
    object-fit: cover;
    background-repeat: no-repeat;
    background-position: right;
    background-image: url(./img/dc-logo-bg.png);
}

i {
    color: gray;
    font-size: 2rem;
    margin-right: 1rem;
}

i:hover {
    color: #3682f3;
}

.col h4 {
    padding-bottom: 0.5rem;
}

.col a {
    text-decoration: none;
    color: rgb(146, 146, 146);
    font-size: 0.75rem;
    padding-top: 0.5rem;
}

.thirdSection {
    color: white;
    background-color: black;
    height: 6rem;
}

.third_sec_wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 75%;
    height: 100%;
    margin: 0 auto;
}

.sing_up {
    border: 1px solid #3682f3;
    padding: 0.75rem;
    margin-left: 1rem;
    font-size: 1.25rem;
}

.sing_up:hover {
    background-color: #3682f3;
}

.follow_us {
    display: flex;
    align-items: center;
    gap: 2rem;
    color: #3682f3;
}
</style>

