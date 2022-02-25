<template>
    <div class="card mb-3">
        <h3 class="card-header">{{header}}</h3>
        <div class="img">
            <div class="blur">
                <img :src="image" alt="" class="top">
            </div>
            <img :src="image" alt="" class="backdrop">
        </div>
        <div class="card-body">
            <p class="card-text">{{cardText}}</p>
        </div>
            <h5>post made by: <span class="red">{{name}}</span></h5>
        <div class="card-footer text-muted">{{date}}</div>
    </div>    
</template>

<script>
export default {
    props: {
        header: String,
        cardText: String,
        image: String,
        date: String,
        name: String,
    }
}
</script>

<style scoped>
    div {
        width: 100%;
        overflow: hidden;
    }

    .card {
        width: 100%;
        background-image: linear-gradient(149deg,rgba(255, 255, 255, 0.2),#00000050);
        backdrop-filter: blur(3px);
    }

    .top {
        width: auto;
        height: 50vh;
        display: block;
        margin: 10px auto 10px auto;
        z-index: 1;
    }

    .img {
        transition: 0.3s;
        padding: 10px;
    }

    .img:hover {
        /* background-color: rgba(0,0,0,0.1); */
        background-color:#ffffff13;
        transition: 0.3s;
    }

    h5 {
        color: rgba(255, 255, 255, 0.438);
    }

    .backdrop {
        position: absolute;
        left: 0;
        top: 10%;
        z-index: -1;
        height: 50vh;
        width: 100%;
        filter: blur(20px);
        opacity: 0.5;        
    }

    h3 {
        font-family: 'Bebas Neue', cursive;
        font-weight: 400;
        font-size: 3rem;
    }

    .card-header {
        padding: 5px;
    }

    @media only screen and (max-width: 1400px) {
        .card {
            width: auto;
            padding: 10px;
        }
    }
</style>