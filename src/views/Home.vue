<template>
  <div id="home">
    <div id="intro">
      <Intro greeting="Hi, I'm Nate." description="A web developer" />
    </div>
    <div id="skills">
      <Skills />
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Intro from "@/components/Intro.vue";
import Skills from "@/components/Skills.vue";

export default {
  name: "Home",
  components: {
    Intro,
    Skills
  }
};
</script>

<style scoped>
#home {
  display: flex;
  flex-direction: row;
  font-family: "Anton", sans-serif;
  justify-content: space-between;
  margin: 75px;
}

#intro {
  width: 50%;
  font-size: 80px;
  border-right: 1px solid lightgrey;
}

#skills {
  text-align: left;
  width: 50%;
  margin-left: 10%;
}

@media screen and (max-width: 975px) {
  #home {
    flex-direction: column;
    text-align: center;
    margin: 30px;
  }

  #intro {
    width: 100%;
    border-right: 0px;
    border-bottom: 1px solid lightgrey;
    margin: 10px;
  }

  #skills {
    width: 100%;
    margin: 0;
    text-align: center;
  }

  #skills ul {
    list-style-type: none;
  }
}

@media screen and (max-width: 475px) {
  #home {
    margin: 5px;
  }

  #intro {
    font-size: 50px;
  }

  .skills {
    font-size: 50px;
  }

  li {
    font-size: 25px;
  }
}
</style>
