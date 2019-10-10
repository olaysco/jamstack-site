<template>
  <section>
    <h2 v-text="title"></h2>
  </section>
</template>

<script>
export default {
  data() {
    return {
      title: "THE CODE LION"
    };
  }
};
</script>

<style lang="scss" scoped>
@import "@/assets/mixins.scss";

section {
  width: 100%;
  height: 30vw;
  overflow: hidden;
  background: -moz-radial-gradient(
      center,
      ellipse cover,
      rgba(0, 0, 0, 0) 0%,
      rgba(0, 0, 0, 0) 37%,
      rgba(0, 0, 0, 0.65) 100%
    ),
    url("/lion.jpg") no-repeat center center scroll; /* FF3.6-15 */
  background: -webkit-radial-gradient(
      center,
      ellipse cover,
      rgba(0, 0, 0, 0) 0%,
      rgba(0, 0, 0, 0) 37%,
      rgba(0, 0, 0, 0.65) 100%
    ),
    url("/lion.jpg") no-repeat center center scroll; /* Chrome10-25,Safari5.1-6 */
  background: radial-gradient(
      ellipse at center,
      rgba(0, 0, 0, 0) 0%,
      rgba(0, 0, 0, 0) 37%,
      rgba(0, 0, 0, 0.65) 100%
    ),
    url("/lion.jpg") no-repeat center center scroll; /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
  background-size: cover;
  color: #FFF;
  h1 {
    margin-top: 0.5em;
    @include fluid-type(font-size, 320px, 1366px, 30px, 100px);
  }
  h2 {
    margin-top: 0;
    padding-top: 1em;
    @include fluid-type(font-size, 320px, 1366px, 15px, 60px);
  }
}
</style>
