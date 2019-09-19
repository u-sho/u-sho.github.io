<template>
  <div>
    <Header />
    <section class="main-content columns">
      <aside class="column is-2 section">
        <p class="menu-label is-hidden-touch">
          General
        </p>
        <ul class="menu-list">
          <li v-for="(item, key) of items" :key="key">
            <nuxt-link :to="item.to" exact-active-class="is-active">
              <b-icon :icon="item.icon" /> {{ item.title }}
            </nuxt-link>
          </li>
        </ul>
      </aside>

      <div class="container column is-10">
        <nuxt />
      </div>
    </section>
    <Footer />
  </div>
</template>

<script>
export default {
  components: {
    Header: () => import('~/components/molecules/Header'),
    Footer: () => import('~/components/molecules/Footer')
  },
  data() {
    return {
      items: [
        {
          title: 'Home',
          icon: 'home',
          to: { name: 'index' }
        },
        {
          title: 'Buefy',
          icon: 'view-dashboard',
          to: { name: 'buefy' }
        }
      ]
    }
  }
}
</script>
