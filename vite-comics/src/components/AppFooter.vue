<script>
export default {

}
</script>

<template>
  <footer>
    <!-- Inizio Section Footer Menu -->
    <div class="section-footer-menu">
      <div class="container">
        <!-- Inizio Footer Menu -->
        <div class="footer-menu">
          <div class="menu-list">
            <h3> Dc Comics</h3>

            <ul>
              <li>Characters</li>
              <li>Comics</li>
              <li>Movies</li>
              <li>Tv</li>
              <li>Games</li>
              <li>Videos</li>
              <li>News</li>
            </ul>
          </div>

          <div class="menu-list">
            <h3>Dc</h3>

            <ul>
              <li>Term of Use</li>
              <li>Privacy Policy (New)</li>
              <li>Ad Choise</li>
              <li>Advertising</li>
              <li>Job</li>
              <li>Subscriptions</li>
              <li>Talent Workshop</li>
              <li>CPSC Certificates</li>
              <li>Ratings</li>
              <li>Shop Help</li>
              <li>Contact Us</li>
            </ul>
          </div>

          <div class="menu-list">
            <h3>Sites</h3>

            <ul>
              <li>DC</li>
              <li>MAD Magazine</li>
              <li>DC Kids</li>
              <li>DC Universe</li>
              <li>DC Power Visa</li>
            </ul>
          </div>

        </div>
        <!-- Fine Footer Menu -->
      </div>
    </div>
    <!-- Fine Section -->
  </footer>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

.section-footer-menu {
  background-image: url('/images/footer-bg.jpg');
  padding: 30px 0;
}

.footer-menu {
  display: flex;
  gap: 40px;
}

.menu-list {

  h3 {
    color: white;
    text-transform: uppercase;
    margin-bottom: 15px;
  }

  ul {
    color: $color-menuitem-footer;

    li {
      margin-bottom: 5px;
    }
  }

}
</style>