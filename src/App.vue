<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Movie</router-link>
      <router-link to="/shows">TV Show</router-link>
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
#app {
  height: 100vh;
  overflow: hidden;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

#nav {
  margin: 0 auto;
  width: 20vw;
  padding: 30px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;

  a {
    color: #707070;
    text-transform: uppercase;
    letter-spacing: 3px;
    font-family: 'Chivo', sans-serif;

    &.router-link-exact-active {
      color: #000000;
      text-decoration: underline;
    }
  }
}

.btn-secondary {
    color: #fff!important;
    background-color: #707070!important;
    border-color: transparent!important;
    font-family: 'Chivo', sans-serif!important;

    &:hover {
      background-color: #000000!important;
    }
}

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
  color: #707070;
}

.movie, .show { 
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

    .transcriptContainer {
      text-align: left;

      .transcriptText {
        padding: 30px 20px;
        margin-bottom: 25px;
        height: 430px;
        text-align: left;
        overflow: scroll;
        -webkit-box-shadow: 0px 0px 53px -17px rgba(0,0,0,0.47);
        -moz-box-shadow: 0px 0px 53px -17px rgba(0,0,0,0.47);
        box-shadow: 0px 0px 53px -17px rgba(0,0,0,0.47);

        .duration {
          background-color: #F2F2F2;
          color: #707070;
          padding: 10px;
          margin: 10px 0;
          font-family: 'Space Mono', monospace;
          // display: block;
        }

        p {
          margin: 15px 0;
          font-family: 'Chivo', sans-serif;
          color: #000000;
        }
      }
    }
  }
}
</style>
