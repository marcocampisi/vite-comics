<script>
import Comic from './Comic.vue';

export default {
  data() {
    return {
      comics: [
        {
          "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
          "price": "$19.99",
          "series": "Action Comics",
          "type": "comic book",
        },
        {
          "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
          "price": "$3.99",
          "series": "American Vampire 1976",
          "type": "comic book",
        },
        {
          "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
          "price": "$16.99",
          "series": "Aquaman",
          "type": "graphic novel",
        },
        {
          "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
          "price": "$2.99",
          "series": "Batgirl",
          "type": "comic book",
        },
        {
          "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
          "price": "$3.99",
          "series": "Batman",
          "type": "comic book",
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
          "price": "$2.99",
          "series": "Batman Beyond",
          "type": "comic book",
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
          "price": "$3.99",
          "series": "Batman/Superman",
          "type": "comic book",
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
          "price": "$4.99",
          "series": "Batman/Superman Annual",
          "type": "comic book",
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
          "price": "$5.99",
          "series": "Batman: The Joker War Zone",
          "type": "comic book",
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
          "price": "$6.99",
          "series": "Batman: Three Jokers",
          "type": "comic book",
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
          "price": "$4.99",
          "series": "Batman: White Knight Presents: Harley Quinn",
          "type": "comic book",
        },
        {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
          "price": "$16.99",
          "series": "Catwoman",
          "type": "graphic novel",
        },
      ]
    }
  },
  components: {
    Comic
  }
}
</script>

<template>
  <div class="mainContainer">
    <div class="topContent">
      <h2>CURRENT SERIES</h2>
      <div class="comicsContainer">
        <Comic v-for="(comic, comicIndex) in comics" :key="comicIndex" :comicThumb="comic.thumb"
          :comicSeries="comic.series" />
      </div>
      <button>LOAD MORE</button>
    </div>
    <div class="midContent">
      <div class="midContainer">
        <div class="midLink">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          <span>DIGITAL COMICS</span>
        </div>
        <div class="midLink">
          <img src="../assets/img/buy-comics-merchandise.png" alt="">
          <span>DC MERCHANDISE</span>
        </div>
        <div class="midLink">
          <img src="../assets/img/buy-comics-subscriptions.png" alt="">
          <span>SUBSCRIPTION</span>
        </div>
        <div class="midLink">
          <img src="../assets/img/buy-comics-shop-locator.png" alt="">
          <span>COMIC SHOP LOCATOR</span>
        </div>
        <div class="midLink">
          <img src="../assets/img/buy-dc-power-visa.svg" alt="">
          <span>DC POWER VISA</span>
        </div>
      </div>
    </div>
    <div class="botContent">
      <div class="dc-logo"></div>
      <div class="linksCol">
        <h3>DC COMICS</h3>
        <p>Characters</p>
        <p>Comics</p>
        <p>Movies</p>
        <p>TV</p>
        <p>Games</p>
        <p>Videos</p>
        <p>News</p>
        <h3>SHOP</h3>
        <p>Shop DC</p>
        <p>Shop DC Collectibles</p>
      </div>
      <div class="linksCol">
        <h3>DC</h3>
        <p>Terms Of Use</p>
        <p>Privacy policy (new)</p>
        <p>Ad Choices</p>
        <p>Advertising</p>
        <p>Jobs</p>
        <p>Subscriptions</p>
        <p>Talent Workshops</p>
        <p>CPSC Certificates</p>
        <p>Ratings</p>
        <p>Shop Help</p>
        <p>Contact Us</p>
      </div>
      <div class="linksCol">
        <h3>SITES</h3>
        <p>DC</p>
        <p>MAD Magazine</p>
        <p>DC Kids</p>
        <p>DC Universe</p>
        <p>DC Power Visa</p>
      </div>
    </div>
  </div>
</template>

<style scoped></style>