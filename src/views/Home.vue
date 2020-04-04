<template>
  <div class="home">
    <Video />
  </div>
</template>

<script>
// @ is an alias to /src
import Video from "@/components/Video.vue";

export default {
  name: "Home",
  components: {
    Video
  }
};
</script>

<style lang="scss">
.home {
  display: flex;
  flex-direction: column;
  align-content: center;
  justify-content: center;
}
</style>
