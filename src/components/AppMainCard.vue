<template>
  <div class="album">
      <img :src="responseObj.poster" alt="">
      <h4>{{ responseObj.title }}</h4>
      <h5>{{ responseObj.author }}</h5>
      <h5>{{ responseObj.year }}</h5>
  </div>
</template>

<script>
export default {
    name: "AppMainCard",
    props: ["responseObj"]

}
</script>

<style lang="scss" scoped>
.album {
    width: calc(100%/5 - 6px);
    background-color: blueviolet;
    padding: 0.5rem;
    margin: 3px;

    img {
        width: 100%;
    }
}

</style>