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
    margin: 1rem;
    gap: 10rem;
    font-size: 0.85rem;

}


.titles a {
    text-decoration: none;
    color: black;
    font-weight: bold;
    cursor: pointer;
    padding-bottom: 1rem;
    padding: 1rem;
}

.titles>a:hover {
    color: #3682f3;
    border-bottom: 4px solid #3682f3;
}

.navbar img {
    padding-right: 5rem;
    width: 10rem;
}
</style>