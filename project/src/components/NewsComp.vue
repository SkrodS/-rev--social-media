<template>
   <div class="box">
        <h1>News</h1>
        <hr>
        <VueRssFeed :feedUrl="feedUrl" :name="name" :limit="limit"/>
   </div>
</template>

<script>
import VueRssFeed from "vue-rss-feed";

export default {
    name: "DEMO",
    components: {
        VueRssFeed
    },
    data() {
        return {
            feedUrl: "https://rss.app/feeds/hmsyAr3PyniBpmOd.xml",
            name: "",
            limit: 5,
        };
    },
}
</script>

<style scoped>
    h1 {
        color: White;
    }

    div {
        color: white;
    }

    hr {
        color: rgba(188, 50, 35, 0.671);
        margin-top: 0;
        margin-bottom: 0.9375rem;
        height: 1px;
    }

    h1 {
        font-family: 'Bebas Neue', cursive;
        font-weight: 400;
        font-size: 5rem;
        margin: 0;
    }

    .box {
        display: box;
        margin: 0 0 0 auto;
        border-radius: 10px;
        background: rgba(188,51,35,0.3);
        -webkit-backdrop-filter: blur(3px);
        backdrop-filter: blur(1px);
        border: 1px solid rgba(188,51,35,0.15);
        width: 100%;
        padding: 2%;

        /* -webkit-box-shadow: 0 0 32px -8px #bc3323;
        -moz-box-shadow: 0 0 32px -8px #bc3323;
        box-shadow: 0 0 32px -8px #bc3323; */
    }
</style>