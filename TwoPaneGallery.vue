<template>
  <div class="gallery
  ">
  <h1 class="sectionName">EXPLORE THE COLLECTION</h1>
  <div class="cards">
  <b-row>
   <b-col class="firstCard cardStyles mr-md-1"></b-col>
   <b-col class="secondCard cardStyles mr-md-1"></b-col>
   <b-col class="thirdCard cardStyles mr-md-1"></b-col>
   <b-col class="fourthCard cardStyles mr-md-1"></b-col>
  </b-row>
  <b-row>
   <b-col> {{ captionOne }} <i class="fas fa-chevron-right"></i></b-col>
   <b-col> {{ captionTwo }} <i class="fas fa-chevron-right"></i> </b-col>
   <b-col> {{ captionThree }} <i class="fas fa-chevron-right"></i></b-col>
   <b-col> {{ captionFour }} <i class="fas fa-chevron-right"></i></b-col>
  </b-row>
  </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      captionOne: 'FAVORITES',
      captionTwo: 'NEW',
      captionThree: 'HANGING',
      captionFour: 'WALL'
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}

.sectionName {
  padding-top: 2.5em;
  padding-bottom: 2em;
  display:flex;
  justify-content:center;
  font-size: 1.5em;
  font-family: 'Catamaran', sans-serif;
}

.bv-example-row {
  padding-top:2em;
  display:flex;
  
}

.row {
  height: 26.5em;
}

.cards {
  margin-right: 2em;
}

.cardStyles {
height: 35em;
background-repeat: no-repeat;
padding: -10em;
margin-left: 2%;
}

.firstCard {
background-image: url('~@/assets/tallBannerFirstCard.png');
}

.secondCard {
background-image: url('~@/assets/tallBannerSecondCard.png');
}

.thirdCard {
background-image: url('~@/assets/tallBannerThirdCard.png');
}

.fourthCard {
background-image: url('~@/assets/tallBannerFourthCard.png');
}

</style>
