<template>
  <div class="home">
    <div class="header">
      <div class="hd1">
        <span class="font4 navGrey hd1">news<span  class="font4 blue">COVID</span></span>
      </div>
    </div>
    <br><br><br>
    <div class="general">
      <div class="grid-container">
        <div class="color1 grid-item item1">
          <h5> <a v-bind:href="newsData.news.data[0].url" target="_blank"> {{ newsData.news.data[0].title }} </a> </h5>
          <h5><a v-bind:href="newsData.news.data[0].sourceURL" target="_blank"> {{ newsData.news.data[0].source }}</a> </h5>
        </div>
        <div class="color1 grid-item item2">
          <h5> <a v-bind:href="newsData.news.data[1].url" target="_blank"> {{ newsData.news.data[1].title }} </a></h5>
          <h5> <a v-bind:href="newsData.news.data[1].sourceURL" target="_blank"> {{ newsData.news.data[1].source }}</a> </h5>
        </div>
        <div class="color1 grid-item item3">
          <h5> <a v-bind:href="newsData.news.data[2].url" target="_blank"> {{ newsData.news.data[2].title }} </a></h5>
          <h5> <a v-bind:href="newsData.news.data[2].sourceURL" target="_blank"> {{ newsData.news.data[2].source }}</a> </h5>
        </div>
        <div class="color1 grid-item item4">
          <h5> <a v-bind:href="newsData.news.data[3].url" target="_blank"> {{ newsData.news.data[3].title }} </a></h5>
          <h5> <a v-bind:href="newsData.news.data[3].sourceURL" target="_blank"> {{ newsData.news.data[3].source }}</a> </h5>
        </div>
      </div>
      <div class="ggrid-container">
      <div class="color1 gitem2">
        <h5> <a v-bind:href="newsData.news.data[4].url" target="_blank"> {{ newsData.news.data[4].title }} </a></h5>
        <h5> <a v-bind:href="newsData.news.data[4].sourceURL" target="_blank"> {{ newsData.news.data[4].source }}</a> </h5>
      </div>
      <div class="color1 gitem3">
        <h5> <a v-bind:href="newsData.news.data[5].url" target="_blank"> {{ newsData.news.data[5].title }} </a></h5>
        <h5> <a v-bind:href="newsData.news.data[5].sourceURL" target="_blank"> {{ newsData.news.data[5].source }}</a> </h5>
      </div>
      <div class="color1 gitem4">
        <h5> <a v-bind:href="newsData.news.data[6].url" target="_blank"> {{ newsData.news.data[6].title }} </a></h5>
        <h5> <a v-bind:href="newsData.news.data[6].sourceURL" target="_blank"> {{ newsData.news.data[6].source }}</a> </h5>
      </div>
      <div class="color1 gitem5">
        <h5> <a v-bind:href="newsData.news.data[7].url" target="_blank"> {{ newsData.news.data[7].title }} </a></h5>
        <h5> <a v-bind:href="newsData.news.data[7].sourceURL" target="_blank"> {{ newsData.news.data[7].source }}</a> </h5>
      </div>
    </div>
    </div>
    <br><br>

    <div class="vt">
    <div class="vaccine">
      <h1 class="title_color aoc"> Vaccine news </h1>
      <div class="snews">
        <h4 class="aoc">
          <span class="title_color"> 1. </span>
          <a v-bind:href="newsData.vaccine.data[0].url" target="_blank"> {{ newsData.vaccine.data[0].title }} </a>
        </h4>
        <h4>
          <span class="title_color"> Source: </span>
          <a v-bind:href="newsData.vaccine.data[0].sourceURL" target="_blank"> {{ newsData.vaccine.data[0].source }}</a>
        </h4>
      </div>
      <div class="snews">
        <h4 class="aoc">
          <span class="title_color"> 2. </span>
          <a v-bind:href="newsData.vaccine.data[1].url" target="_blank"> {{ newsData.vaccine.data[1].title }} </a>
        </h4>
        <h4>
          <span class="title_color"> Source: </span>
          <a v-bind:href="newsData.vaccine.data[1].sourceURL" target="_blank"> {{ newsData.vaccine.data[1].source }}</a>
        </h4>
      </div>
      <div class="snews">
        <h4 class="aoc">
          <span class="title_color"> 3. </span>
          <a v-bind:href="newsData.vaccine.data[2].url" target="_blank"> {{ newsData.vaccine.data[4].title }} </a>
        </h4>
        <h4>
          <span class="title_color"> Source: </span>
          <a v-bind:href="newsData.vaccine.data[2].sourceURL" target="_blank"> {{ newsData.vaccine.data[2].source }}</a>
        </h4>
      </div>
      <div class="snews">
        <h4 class="aoc">
          <span class="title_color"> 4. </span>
          <a v-bind:href="newsData.vaccine.data[3].url" target="_blank"> {{ newsData.vaccine.data[4].title }} </a>
        </h4>
        <h4>
        <span class="title_color"> Source: </span>
        <a v-bind:href="newsData.vaccine.data[3].sourceURL" target="_blank"> {{ newsData.vaccine.data[3].source }}</a>
        </h4>
      </div>
      <div class="snews">
        <h4 class="aoc">
          <span class="title_color"> 5. </span>
          <a v-bind:href="newsData.vaccine.data[4].url" target="_blank"> {{ newsData.vaccine.data[4].title }} </a>
        </h4>
        <h4>
          <span class="title_color"> Source: </span>
          <a v-bind:href="newsData.vaccine.data[4].sourceURL" target="_blank"> {{ newsData.vaccine.data[4].source }}</a>
        </h4>
      </div>
    </div>

    <div class="treatment">
      <h1 class="title_color aoc"> Treatment news </h1>
      <div class="snews">
        <h4 class="aoc">
          <span class="title_color"> 1. </span>
          <a v-bind:href="newsData.treament.data[0].url" target="_blank"> {{ newsData.treament.data[0].title }} </a>
        </h4>
        <h4>
          <span class="title_color"> Source: </span>
          <a v-bind:href="newsData.treament.data[0].sourceURL" target="_blank"> {{ newsData.treament.data[0].source }}</a>
        </h4>
      </div>
      <div class="snews">
        <h4 class="aoc">
          <span class="title_color"> 2. </span>
          <a v-bind:href="newsData.treament.data[1].url" target="_blank"> {{ newsData.treament.data[1].title }} </a>
        </h4>
        <h4>
          <span class="title_color"> Source: </span>
          <a v-bind:href="newsData.treament.data[1].sourceURL" target="_blank"> {{ newsData.treament.data[1].source }}</a>
        </h4>
      </div>
      <div class="snews">
        <h4 class="aoc">
          <span class="title_color"> 3. </span>
          <a v-bind:href="newsData.treament.data[2].url" target="_blank"> {{ newsData.treament.data[2].title }} </a>
        </h4>
        <h4>
          <span class="title_color"> Source: </span>
          <a v-bind:href="newsData.treament.data[2].sourceURL" target="_blank"> {{ newsData.treament.data[2].source }}</a>
        </h4>
      </div>
      <div class="snews">
        <h4 class="aoc">
          <span class="title_color"> 4. </span>
          <a v-bind:href="newsData.treament.data[3].url" target="_blank"> {{ newsData.treament.data[3].title }} </a>
        </h4>
        <h4>
          <span class="title_color"> Source: </span>
          <a v-bind:href="newsData.treament.data[3].sourceURL" target="_blank"> {{ newsData.treament.data[3].source }}</a>
        </h4>
      </div>
      <div class="snews">
        <h4 class="aoc">
          <span class="title_color"> 5. </span>
          <a v-bind:href="newsData.treament.data[4].url" target="_blank"> {{ newsData.treament.data[4].title }} </a>
        </h4>
        <h4>
          <span class="title_color"> Source: </span>
          <a v-bind:href="newsData.treament.data[4].sourceURL" target="_blank"> {{ newsData.treament.data[4].source }}</a>
        </h4>
      </div>
    </div>
  <!-- end of vt -->
  </div>
  <br><br>
  <div class="footer">
    <span class="navGrey">
      .: created by Iordanis Paschalidis
    </span>
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

.general{
  position: relative;
  width : 90%;
  left: 5%;
  top: 10%;
}

body{
  background-color: #181b1e;
}

.color1{
  background-color: #327ba5;
}

a{
  color:white;
}

.title_color{
  color:#d17402;
}

.aoc{
  text-align: left;
}

.snews{
  width : 90%;
}

.item1 {
  grid-column: 1 / span 2;
  grid-row: 1;
  transition: transform .2s; /* Animation */
}

.item1:hover {
  background-color: #154561;
  transform: scale(1.1); /* (150% zoom - Note: if the zoom is too large, it will go outside of the viewport) */
}

.item2 {
  grid-column: 3;
  grid-row: 1 / span 2;
  transition: transform .2s; /* Animation */
}

.item2:hover {
  background-color: #154561;
  transform: scale(1.1); /* (150% zoom - Note: if the zoom is too large, it will go outside of the viewport) */
}

.item3 {
  transition: transform .2s; /* Animation */
}

.item3:hover {
  background-color: #154561;
  transform: scale(1.1); /* (150% zoom - Note: if the zoom is too large, it will go outside of the viewport) */
}

.item4 {
  transition: transform .2s; /* Animation */
}

.item4:hover {
  background-color: #154561;
  transform: scale(1.1); /* (150% zoom - Note: if the zoom is too large, it will go outside of the viewport) */
}

.item5 {
  grid-column: 1 / span 3;
  grid-row: 3;
  transition: transform .2s; /* Animation */
}

.item5:hover {
  background-color: #154561;
  transform: scale(1.1); /* (150% zoom - Note: if the zoom is too large, it will go outside of the viewport) */
}

.gitem1 {
  grid-area: myArea;
  grid-gap: 2px;
  padding: 2px;
  transition: transform .2s; /* Animation */
}

.gitem1:hover {
  background-color: #154561;
  transform: scale(1.1); /* (150% zoom - Note: if the zoom is too large, it will go outside of the viewport) */
}

.gitem2 {
  transition: transform .2s; /* Animation */
}

.gitem2:hover {
  background-color: #154561;
  transform: scale(1.1); /* (150% zoom - Note: if the zoom is too large, it will go outside of the viewport) */
}

.gitem3 {
  transition: transform .2s; /* Animation */
}

.gitem3:hover {
  background-color: #154561;
  transform: scale(1.1); /* (150% zoom - Note: if the zoom is too large, it will go outside of the viewport) */
}

.gitem4 {
  transition: transform .2s; /* Animation */
}

.gitem4:hover {
  background-color: #154561;
  transform: scale(1.1); /* (150% zoom - Note: if the zoom is too large, it will go outside of the viewport) */
}

.gitem5 {
  transition: transform .2s; /* Animation */
}

.gitem5:hover {
  background-color: #154561;
  transform: scale(1.1); /* (150% zoom - Note: if the zoom is too large, it will go outside of the viewport) */
}

.ggrid-container {
  display: grid;
  grid-template-areas: 'myArea myArea myArea myArea';
  grid-gap: 2px;
}

.ggrid-container > div {
  text-align: center;
  padding: 20px;
  font-size: 20px;
}

.grid-container {
  display: grid;
  grid-gap: 2px;
  padding: 2px;
}

.grid-item {
  text-align: center;
  padding: 20px;
  font-size: 20px;
}

.vt {
  display: flex;
  justify-content: center;
}

.font4{
  font-style: normal;
  font-weight: 600;
  font-size: 30px;
  font-size: 3vw;
}

.navGrey{
  color: white;
}
.blue{
  color: #154561;
}
.header{
  text-align: left;
}

.footer {
  left: 0;
  bottom: 0;
  width: 100%;
  background-color: #154561;
  text-align: center;
  height: 50px;
}

</style>
