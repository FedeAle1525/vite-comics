<script>
export default {

  data() {
    return {
      menus: [
        {
          title: 'Dc Comics',
          items: ['Character', 'Comics', 'Movies', 'Tv', 'Games', 'Videos', 'News']
        },
        {
          title: 'Dc',
          items: ['Term of Use', 'Privacy Policy (New)', 'Ad Choise', 'Advertising', 'Job', 'Subscriptions', 'Talent Workshop',
            'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us']
        },
        {
          title: 'Sites',
          items: ['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']
        }
      ]
    }
  }
}
</script>

<template>
  <footer>
    <!-- Inizio Section Footer Menu -->
    <div class="section-footer-menu">
      <div class="container">
        <!-- Inizio Footer Menu -->
        <div class="footer-menu">

          <div class="menu-list" v-for="(menu, i) in menus" :key="i">
            <h3>{{ menu.title }}</h3>

            <ul>
              <li v-for="(item, j) in menu.items" :key="j">
                {{ item }}
              </li>
            </ul>
          </div>

        </div>
        <!-- Fine Footer Menu -->
      </div>
    </div>
    <!-- Fine Section Footer Menu -->

    <section class="section-footer-credits">
      <div class="container">
        <div class="footer-credits">

          <div class="button">
            Sign-up now!
          </div>

          <div class="menu-icons">
            <h3>Follow Us</h3>

            <ul>
              <li>
                <img src="/images/footer-facebook.png" alt="">
              </li>
              <li>
                <img src="/images/footer-twitter.png" alt="">
              </li>
              <li>
                <img src="/images/footer-youtube.png" alt="">
              </li>
              <li>
                <img src="/images/footer-pinterest.png" alt="">
              </li>
              <li>
                <img src="/images/footer-periscope.png" alt="">
              </li>
            </ul>
          </div>
        </div>

      </div>
    </section>
  </footer>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

// FOOTER-MENU
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

// FOOTER CREDITS
.section-footer-credits {
  padding: 30px;
  background-color: $bg-footer-credits;
}

.footer-credits {
  display: flex;
  justify-content: space-between;
  align-items: center;

  .button {
    color: white;
    text-transform: uppercase;
    border: 2px solid $color-activate-link;
    padding: 0 10px;
    line-height: 40px;
  }

  .menu-icons {
    display: flex;
    align-items: center;
    gap: 25px;

    h3 {
      color: $color-activate-link;
      text-transform: uppercase;
    }

    ul {
      display: flex;
      gap: 15px;
    }
  }
}
</style>