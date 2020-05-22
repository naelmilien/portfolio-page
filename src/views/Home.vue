<template>
  <div id="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png" /> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <div id="intro">
      <p class="intro">
        Hi, I'm Nate.
        <br />
        <span class="job-title">A web developer</span>.
      </p>
    </div>
    <div id="skills">
      <h1 class="skills">Skills</h1>
      <ul>
        <li>Front End Web Development</li>
        <li>Back-End Web Development</li>
        <li>Full-Stack Web Development</li>
        <li>Test-Driven Development</li>
        <li>Pair Programming</li>
        <li>Agile Software Development</li>
      </ul>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";

// export default {
//   name: "Home",
//   components: {
//     HelloWorld
//   }
// };
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

.job-title {
  color: #8bf98b;
}

#skills {
  text-align: left;
  width: 50%;
  margin-left: 10%;
}

.skills {
  color: #8bf98b;
  font-size: 60px;
  text-decoration: underline;
  text-decoration-color: #5e5b5e;
  width: 50%;
  font-weight: lighter;
  margin-bottom: 0px;
}

#skills ul {
  margin: 0px;
  font-size: 30px;
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

  .skills {
    text-align: center;
    margin: 10px auto;
  }

  #skills ul {
    list-style-type: none;
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
}
</style>
