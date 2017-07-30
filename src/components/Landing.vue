<template lang="pug">
  div
    #intro
      v-container(fluid).elevation-8
        v-layout(row wrap justify-center)
          v-flex(xs12).text-xs-center
            h2.white--text StreetTraffic.org
            h6.white--text Monitor the traffic flow of your favorite routes, cities and more!
            div.mt-5
              v-btn(light large tag="a" href="https://github.com/streettraffic/streettraffic").grey.lighten-2 Github
              v-btn(light large tag="a" href="https://streettraffic.github.io/docs/docindex.html").green.lighten-2 Get Started

    #feature
      v-container(fluid).mt-5
        v-layout(row wrap justify-center align-center)
          v-flex(xs12 md5)
            v-card.transparent.elevation-0.pa-3
              v-card-title.pl-0.pt-0.headline See the traffic flow history!
              div.grey--text.text--darken-1 
              |StreetTraffic enables you to query the history traffic flow data
              |with respect to a particular route.

          v-flex(xs12 md5)
            v-card(img="/static/TrafficFlowQuery.gif" height="500px" slot="activator")

      v-container(fluid).mt-5
        v-layout(row wrap justify-center align-center)
          v-flex(xs12 md5)
            v-card(img="/static/TrafficPattern.gif" height="500px" slot="activator")
          v-flex(xs12 md5)
            v-card.transparent.elevation-0.pa-3
              v-card-title.pl-0.pt-0.headline Query the traffic pattern of a region!
              div.grey--text.text--darken-1 
              |You may sample many roads within a given region and calculate
              |the average jamming factor(a measurement of traffic flow) of those roads

      v-container(fluid).mt-5
        v-layout(row wrap justify-center align-center)
          v-flex(xs12 md5)
            v-card.transparent.elevation-0.pa-3
              v-card-title.pl-0.pt-0.headline Directly mess with database!
              div.grey--text.text--darken-1 
              |StreetTraffic uses RethinkDB as its datastore, which 
              |is very easy to setup and do queries.

          v-flex(xs12 md5)
            v-card(img="/static/RethinkDB.gif" height="500px" slot="activator")


      v-container(fluid).mt-5
        v-layout(row wrap justify-center align-center)
          v-flex(xs12 md5)
            v-card(img="/static/historyBatch.gif" height="500px" slot="activator")
          v-flex(xs12 md5)
            v-card.transparent.elevation-0.pa-3
              v-card-title.pl-0.pt-0.headline Easily manage the data you stored!
              div.grey--text.text--darken-1
              |By using the History Batch route, you can easily 
              |see most recent data download

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

// #303030 
#intro
  
  .container
    padding-top: 15vh
    background-color: #303030
    height: 50vh

    .btn
      display: inline-block
      width: 140px

#feature

  padding
</style>
