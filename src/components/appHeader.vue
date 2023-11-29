<script>

export default {
    name: "appHeader",
    data() {
        return {
            navTitles: [
                {
                    text: "CHARACTERS",
                    link: "#",
                }, {
                    text: "COMICS",
                    link: "#",
                }, {
                    text: "MOVIES",
                    link: "#",
                }, {
                    text: "TV",
                    link: "#",
                }, {
                    text: "GAMES",
                    link: "#",
                }, {
                    text: "COLLECTIBLES",
                    link: "#",
                }, {
                    text: "VIDEOS",
                    link: "#",
                }, {
                    text: "FANS",
                    link: "#",
                }, {
                    text: "NEWS",
                    link: "#",
                }, {
                    text: "SHOP",
                    link: "#",
                }
            ]
        }
    }
}


</script>

<template>
    <div class="wrapper">
        <header>
            <nav class="navbar">
                <img src="/img/dc-logo.png " alt="logo">
                <div class="titles">
                    <a v-for=" title in navTitles " href="title.link">{{ title.text }}</a>
                </div>
            </nav>
        </header>
    </div>
</template>

<style scoped>
.navbar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    font-size: 0.85rem;
    height: 6rem;


}


.titles a {
    text-decoration: none;
    color: black;
    font-weight: bold;
    cursor: pointer;
    margin: 1rem;
}

.titles>a:hover {
    color: #3682f3;
    border-bottom: 7px solid #3682f3;
    padding-bottom: 2.1rem;
}

.navbar img {
    padding-right: 5rem;
    width: 10rem;
}
</style>