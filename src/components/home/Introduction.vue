<template>
  <div id="introduction">
    <div class="overlay">
      <div class='title-text'>
        Hello, I'm <div class='name-highlight'>Lianne Espeland.</div>
      </div>
      <div class='title-text'>I'm a full-stack web developer</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'introduction',
};
</script>

<style lang="sass">
  @import "@/assets/styles/base.sass"
  #introduction
    @supports (-webkit-overflow-scrolling: touch)
      height: 600px
    @supports not (-webkit-overflow-scrolling: touch)
      height: calc(100vh)
  .overlay
    margin-left: auto
    margin-right: auto
    position: absolute
    text-align: center
    left: 0
    right: 0
    color: $white
    margin-top: 250px
    .title-text
      z-index: 1
      font-size: 26px
      .name-highlight
        display: -webkit-inline-box
        color: $pink
</style>
