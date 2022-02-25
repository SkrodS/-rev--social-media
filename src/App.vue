  <template>
  <div id="body">
    <nav-bar/>
    <carousel/>
    <div class="container cont">
      <div class="row">
        <div class="col">
          <div class="cards">
            <card header="BLADEE" cardText="Nice!! Jag elskar blejd omg so hott and cool wowowowowowowo!!! <333333" date="2 days ago" image="https://static.wikia.nocookie.net/hip-hop-music/images/4/45/Bladee.jpeg" name="Skrod"></card>
            <card header="Kvothe from The name of the wind" cardText="epic post yes very nice" date="10 days ago" name="Robin" image="https://c.wallhere.com/photos/51/17/fantasy_art_kvothe_Kingkiller_Chronicles-168234.jpg!d"></card>
            <card header="M@RK" cardText="epic post yes very nice" date="10 days ago" name="Robin" image="https://talenthouse-res.cloudinary.com/image/upload/c_limit,h_1000,w_1000/v1/user-914783/profile/n6hn8mr1fomxvqwmzswp.jpg"></card>
            <card header="bladee again" cardText="epic post yes very nice" date="10 days ago" name="not Robin" image="https://preview.redd.it/mku4ktq0gfu11.jpg?auto=webp&s=0b41f83b0ab0d06b16d227e3b297fb5efdf9e82d"></card>
          </div>
        </div>
        <div class="col">
          <news/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import NavBar from './components/NavBar.vue'
  import Card from './components/CardComp.vue'
  import Carousel from './components/CarouselComp.vue'
  import News from './components/NewsComp.vue'

  export default {
    name: 'App',
    components: {
      NavBar,
      Card,
      Carousel,
      News,
    }
  }
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&display=swap');
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
  }

  .red {
    color: #BC3323;
  }

  #body {
    background-image: url(./assets/background.svg);
    background-position-x: center;
    padding-bottom: 3vh;
  }

  .cards {
    /* position: absolute;
    top: 10%;
    left: 10%; */
    /* margin: 1.25rem; */
    width: fit-content;
  }

  .cont {
    margin-left: auto;
    margin-right: 0 auto 0 auto;
  }

  news {
    display: block;
  }

  .feed {
    color: white;
  }

  .article[data-v-af400700] {
    background-color: #ffffff00;
    transition: 0.4s;
    border: 1px solid rgba(188,51,35,0.15);
  }

  .vue-rss-feed[data-v-0c2deced] {
    display: block;
    margin: 0 auto 0 auto;
  }

  .article[data-v-af400700]:hover {
    background-color:#ffffff13;
    transition: 0.3s;
  }

  .article[data-v-af400700] a {
    color: #ffffff;
  }

  @media only screen and (max-width: 1400px) {
    .cards {
      display: block;
      margin: 0 auto 0 auto;
      width: auto;
    }
    .cont, .container {
      display: block;
      margin: 0 auto 0 auto;
      width: auto;
    }
  }

</style>
