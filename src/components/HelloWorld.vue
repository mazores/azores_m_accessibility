<template>
  <div class="hello">
    <b-container fluid class="compContainer">
      <b-row>
          <b-col m="7" class="videoContainer">
          <iframe class="video" src="https://www.youtube.com/embed/jEDaVHmw7r4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>          
          </b-col>

          <b-col m="5" class="px-5 transcriptContainer">
          <div class="transcriptText">
          <span class="duration">00:00</span>
          Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum.

          <span class="duration">00:00</span>
          Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum.
          </div>
          
          <b-button>
              Download Transcript
          </b-button>
          </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  name: "Video",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
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

.hello { 
  .compContainer {
    .videoContainer {
      position: relative;
      width: 100%;
      height: 500px;
      
      .video { 

        width: 100%;
        height: 100%;

      }
    }
  }
}
</style>
