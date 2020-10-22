<template>
  <div class="home">
    <div class="general">
      <div class="tooltip">
        <span class="tooltiptext">General News </span>
      <div class="grid-container">
        <div class="grid-item item1">
          <h5> {{ newsData.news.data[0].title }} </h5>
          <h5><a v-bind:href="newsData.news.data[0].sourceURL" target="_blank"> {{ newsData.news.data[0].source }}</a> </h5>
        </div>
        <div class="grid-item item2">
          <h5> {{ newsData.news.data[1].title }} </h5>
          <h5> <a v-bind:href="newsData.news.data[1].sourceURL" target="_blank"> {{ newsData.news.data[1].source }}</a> </h5>
        </div>
        <div class="grid-item item3">
          <h5> {{ newsData.news.data[2].title }} </h5>
          <h5> <a v-bind:href="newsData.news.data[2].sourceURL" target="_blank"> {{ newsData.news.data[2].source }}</a> </h5>
        </div>
        <div class="grid-item item4">
          <h5> {{ newsData.news.data[3].title }} </h5>
          <h5> <a v-bind:href="newsData.news.data[3].sourceURL" target="_blank"> {{ newsData.news.data[3].source }}</a> </h5>
        </div>
        <div class="grid-item item5">
          <h5> {{ newsData.news.data[4].title }} </h5>
          <h5> <a v-bind:href="newsData.news.data[4].sourceURL" target="_blank"> {{ newsData.news.data[4].source }}</a> </h5>
        </div>
      </div>
    </div>
    </div>

    <div class="vaccine">
      <div class="tooltip">
        <span class="tooltiptext">Vaccine News </span>
      <div class="grid-container">
        <div class="grid-item item1">
          <h5> {{ newsData.vaccine.data[0].title }} </h5>
          <h5><a v-bind:href="newsData.vaccine.data[0].sourceURL" target="_blank"> {{ newsData.vaccine.data[0].source }}</a> </h5>
        </div>
        <div class="grid-item item2">
          <h5> {{ newsData.vaccine.data[1].title }} </h5>
          <h5> <a v-bind:href="newsData.vaccine.data[1].sourceURL" target="_blank"> {{ newsData.vaccine.data[1].source }}</a> </h5>
        </div>
        <div class="grid-item item3">
          <h5> {{ newsData.vaccine.data[2].title }} </h5>
          <h5> <a v-bind:href="newsData.vaccine.data[2].sourceURL" target="_blank"> {{ newsData.vaccine.data[2].source }}</a> </h5>
        </div>
        <div class="grid-item item4">
          <h5> {{ newsData.vaccine.data[3].title }} </h5>
          <h5> <a v-bind:href="newsData.vaccine.data[3].sourceURL" target="_blank"> {{ newsData.vaccine.data[3].source }}</a> </h5>
        </div>
        <div class="grid-item item5">
          <h5> {{ newsData.vaccine.data[4].title }} </h5>
          <h5> <a v-bind:href="newsData.vaccine.data[4].sourceURL" target="_blank"> {{ newsData.vaccine.data[4].source }}</a> </h5>
        </div>
      </div>
      </div>
    </div>

    <div class="treatment">
      <div class="tooltip">
        <span class="tooltiptext">Treatment News </span>
      <div class="grid-container">
        <div class="grid-item item1">
          <h5> {{ newsData.treament.data[0].title }} </h5>
          <h5><a v-bind:href="newsData.treament.data[0].sourceURL" target="_blank"> {{ newsData.treament.data[0].source }}</a> </h5>
        </div>
        <div class="grid-item item2">
          <h5> {{ newsData.treament.data[1].title }} </h5>
          <h5> <a v-bind:href="newsData.treament.data[1].sourceURL" target="_blank"> {{ newsData.treament.data[1].source }}</a> </h5>
        </div>
        <div class="grid-item item3">
          <h5> {{ newsData.treament.data[2].title }} </h5>
          <h5> <a v-bind:href="newsData.treament.data[2].sourceURL" target="_blank"> {{ newsData.treament.data[2].source }}</a> </h5>
        </div>
        <div class="grid-item item4">
          <h5> {{ newsData.treament.data[3].title }} </h5>
          <h5> <a v-bind:href="newsData.treament.data[3].sourceURL" target="_blank"> {{ newsData.treament.data[3].source }}</a> </h5>
        </div>
        <div class="grid-item item5">
          <h5> {{ newsData.treament.data[4].title }} </h5>
          <h5> <a v-bind:href="newsData.treament.data[4].sourceURL" target="_blank"> {{ newsData.treament.data[4].source }}</a> </h5>
        </div>
      </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from 'axios'

export default {

  data () {
    return {
      newsData: {}
    }
  },
  methods: {
    requestNews () {
      axios.get('http://stats-covid.com/api/news/all')
        .then(response => (
          this.newsData = response.data))
        .catch(function (error) {
          console.log(error)
        })
    }
  },
  mounted () {
    this.requestNews()
  }
}
</script>

<style>
.grid-container {
  display: grid;
  grid-gap: 2px;
  background-color: #2196F3;
  padding: 2px;
}

.grid-item {
  background-color: rgba(255, 255, 255, 0.8);
  text-align: center;
  padding: 20px;
  font-size: 20px;
}

.item1 {
  grid-column: 1 / span 2;
  grid-row: 1;
}

.item2 {
  grid-column: 3;
  grid-row: 1 / span 2;
}

.item5 {
  grid-column: 1 / span 3;
  grid-row: 3;
}

.tooltip .tooltiptext {
  display: flex;
  justify-content: center;
  align-items: center;
  visibility: hidden;
  width: 120px;
  background-color: red;
  color: #fff;
}
.tooltip:hover .tooltiptext {
  visibility: visible;
}
</style>
