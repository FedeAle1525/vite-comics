<script>
export default {

  data() {
    return {
      menuItems: ['Characters', 'Comics', 'Movies', 'Tv', 'Games', 'Collectibles', 'Videos', 'Fans', 'News', 'Shop'],
      indexCurrent: 1,
    }
  },

  methods: {
    changeMenuItem(index) {
      this.indexCurrent = index;
    }
  }
}
</script>

<template>
  <header>
    <div class="container">
      <img src="/images/dc-logo.png" alt="">

      <ul>
        <li v-for="(item, i) in menuItems" :class="(i === indexCurrent) ? 'active' : ''" @click='changeMenuItem(i)'>

          {{ item }}
        </li>
      </ul>
    </div>

  </header>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

header {
  padding: 10px 0;

  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;

    img {
      width: 70px;
    }

    ul {
      display: flex;
      gap: 15px;
      text-transform: uppercase;
      font-size: 14px;

      li.active,
      li:hover {
        color: $color-activate-link;
      }
    }
  }

}
</style>