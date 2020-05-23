<template>
  <p class="intro">
    {{greeting}}
    <br />
    <span class="job-title">{{description}}</span>.
  </p>
</template>

<script>
export default {
  name: "Intro",
  props: {
    greeting: String,
    description: String
  }
};
</script>

<style>
.job-title {
  color: #8bf98b;
}

@media screen and (max-width: 975px) {
  #intro {
    width: 100%;
    border-right: 0px;
    border-bottom: 1px solid lightgrey;
    margin: 10px;
  }
}
</style>