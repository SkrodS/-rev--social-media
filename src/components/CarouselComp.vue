<template>
    <div id="carouselSlidesOnly" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-inner">
            <div class="carousel-item active">
                <img src="https://proletaren.se/sites/default/files/styles/article_full/public/50096105508_169ff4b314_o.jpg?itok=cJd9htfD&timestamp=1594389136" class="d-block w-100" alt="...">
            </div>
            <div class="carousel-item">
                <img src="https://filmcentralen.dk/files/styles/film_teaser/public/dfi_film_images_0/dfi_20191211-170550-5.jpg?itok=ZhY1-Dtp" class="d-block w-100" alt="...">
            </div>
            <div class="carousel-item">
                <img src="http://www.latinamericanstudies.org/peru/rondas.jpg" class="d-block w-100" alt="...">
            </div>
            <h1>f<span class="red">{</span>r<span class="red">}</span>ont page</h1>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
    img {
        height: 45vh;
        object-fit: cover;
        filter: brightness(80%);
    }

    #carouselSlidesOnly {
        height: 48vh;
    }

    h1 {
        margin: 0;
        font-family: 'Bebas Neue', cursive;
        font-size: 8rem;
        font-weight: 400;
        position: absolute;
        right: 1%;
        bottom: -6%;
        color: white;
        transition: 0.4s;
    }

    span {
        transition: 0.4s;
    }

    h1:hover span {
        transition: 0.4s;
        color: white;
    }
    
    h1:hover {
        transition: 0.4s;
        color:#BC3323;
    }
</style>