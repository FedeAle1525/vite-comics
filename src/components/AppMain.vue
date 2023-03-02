<script>
import CardComic from '../components/CardComic.vue';

export default {

  components: {
    CardComic
  },

  data() {
    return {
      comics: [
        {
          thumb: "/images/action-comics.jpg",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book"
        },
        {
          thumb: "/images/american-vampire.jpg",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book"
        },
        {
          thumb: "/images/aquaman.jpg",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel"
        },
        {
          thumb: "/images/batgirl.jpg",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book"
        },
        {
          thumb: "/images/batman.jpg",
          price: "$3.99",
          series: "Batman",
          type: "comic book"
        },
        {
          thumb: "/images/batman-beyond.jpg",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book"
        },
        {
          thumb: "/images/batman-superman.jpg",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book"
        },
        {
          thumb: "/images/batman-superman-annual.jpg",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book"
        },
        {
          thumb: "/images/batman-joker-warzone.jpg",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book"
        },
        {
          thumb: "/images/batman-three-joker.jpg",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book"
        },
        {
          thumb: "/images/harley-queen.jpg",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book"
        },
        {
          thumb: "/images/catwoman.jpg",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel"
        }
      ]
    }
  }
}
</script>

<template>
  <main>
    <div class="container">
      <div class="row">
        <div class="col-6" v-for="(comic, i) in comics" :key="i">
          <!-- <div class="card">
              <img :src="comic.thumb">

              <span>{{ comic.series }}</span>
            </div> -->

          <CardComic :thumb="comic.thumb" :series="comic.series" />
        </div>
      </div>
    </div>
  </main>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

main {
  background-color: $bg-main;
  color: white;
  padding: 40px 0;
}

.row {
  display: flex;
  flex-wrap: wrap;
  margin: 0 -10px;
  row-gap: 30px;

  .col-6 {
    flex-basis: calc(100% / 6);
    padding: 0 10px;
  }


}
</style>