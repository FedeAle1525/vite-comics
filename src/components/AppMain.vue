<script>
export default {

}
</script>

<template>
  <main>
    <div class="container">
      <div class="row">
        <div class="col-6">
          <div class="card">
            <img src="/images/action-comics.jpg">

            <span>Titolo</span>
          </div>
        </div>

        <div class="col-6">
          <div class="card">
            <img src="/images/action-comics.jpg">

            <span>Titolo</span>
          </div>
        </div>

        <div class="col-6">
          <div class="card">
            <img src="/images/action-comics.jpg">

            <span>Titolo</span>
          </div>
        </div>

        <div class="col-6">
          <div class="card">
            <img src="/images/action-comics.jpg">

            <span>Titolo</span>
          </div>
        </div>

        <div class="col-6">
          <div class="card">
            <img src="/images/action-comics.jpg">

            <span>Titolo</span>
          </div>
        </div>

        <div class="col-6">
          <div class="card">
            <img src="/images/action-comics.jpg">

            <span>Titolo</span>
          </div>
        </div>

        <div class="col-6">
          <div class="card">
            <img src="/images/action-comics.jpg">

            <span>Titolo</span>
          </div>
        </div>

        <div class="col-6">
          <div class="card">
            <img src="/images/action-comics.jpg">

            <span>Titolo</span>
          </div>
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

  .card {
    display: flex;
    flex-direction: column;
    gap: 10px;

    img {
      aspect-ratio: 1/1;
      object-fit: cover;
      object-position: top;
    }

    span {
      text-transform: uppercase;
    }
  }
}
</style>