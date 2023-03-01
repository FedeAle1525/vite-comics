<script>
export default {

}
</script>

<template>
  <header>
    <div class="container">
      <img src="/images/dc-logo.png" alt="">

      <ul>
        <li>Characters</li>
        <li class="active">Comics</li>
        <li>Movies</li>
        <li>Tv</li>
        <li>Games</li>
        <li>Collectibles</li>
        <li>Videos</li>
        <li>Fans</li>
        <li>New</li>
        <li>Shop</li>
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