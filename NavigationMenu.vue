<template>
  <div class="gallery">
    <ul class="navRow">
      <li class="icon"><i class="fas fa-bars"></i><i class="fas fa-search" style="padding-left:1em"></i></li>
      <li class=".mx-auto brandName">The Urban Electric Co.</li>
      <li class="login">Log In</li>
    </ul>
  </div>
</template>

<script>
export default {
  brandName: 'The Urban Electric Co.',
  props: {
    msg: String,
  }
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

.navRow {
  display:flex;
  justify-content: space-between;
  align-items: baseline;
  color: #9F9D9E;
}

.brandName {
  font-size: 2em;
  font-family: 'Bitter', serif;
  
}
</style>
