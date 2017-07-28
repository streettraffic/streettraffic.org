<template lang="pug">
  #intro
    v-layout(column align-center justify-center)
      h2.white--text StreetTraffic.org
      h6.white--text Monitor the traffic flow of your favorite routes, cities and more!
      div.mt-5
        v-btn(light large tag="a" href="https://github.com/streettraffic/streettraffic").grey.lighten-2 Github
        v-btn(light large tag="a" href="https://streettraffic.github.io/docs/docindex.html").green.lighten-2 Get Started

</template>

<script>
export default {
  name: 'Landing',
  data () {
    return {
      // pass
    }
  },
  methods: {
    // pass
  }
}
</script>

<style lang="sass">
#intro
  padding-top: 15vh

  .btn
    width: 150px
</style>
