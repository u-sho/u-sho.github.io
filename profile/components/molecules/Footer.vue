<template>
  <footer class="footer is-primary">
    <section class="content">
      <h3 class="has-text-dark">u-sho.github.io</h3>
      <p class="has-text-grey">Copyright © 2019 Shohei Uechi.</p>
    </section>
    <div class="block">
      <a href="https://github.com/u-sho" exact-active-class="is-active">
        <b-icon icon="github-circle" size="is-medium" type="is-dark" />
      </a>
      <a href="https://twitter.com/u_sho_KyoPro" exact-active-class="is-active">
        <b-icon icon="twitter" size="is-medium" type="is-info" />
      </a>
      <a href="mailto:720187sho@gmail.com" exact-active-class="is-active">
        <b-icon icon="gmail" size="is-medium" type="is-danger" />
      </a>
      <a href="https://u-sho.hatenablog.com/" exact-active-class="is-active">
        <HatenaLogo />
      </a>
    </div>
  </footer>
</template>

<script>
export default {
  components: {
    HatenaLogo: () => import('~/components/atoms/HatenablogLogo')
  }
}
</script>
