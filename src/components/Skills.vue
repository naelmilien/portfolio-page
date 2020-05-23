<template>
  <div>
    <h1 class="skills">Skills</h1>
    <ul>
      <li v-for="skill in skills" v-bind:key="skill.text">{{skill.text}}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Skills",
  data: () => {
    return {
      skills: [
        { text: "Front-End Web Development" },
        { text: "Back-End Web Development" },
        { text: "Full-Stack Web Development" },
        { text: "Test Driven Development" },
        { text: "Pair Programming" },
        { text: "Agile Software Development" }
      ]
    };
  }
};
</script>

<style scoped>
.skills {
  color: #8bf98b;
  font-size: 60px;
  text-decoration: underline;
  text-decoration-color: #5e5b5e;
  width: 50%;
  font-weight: lighter;
  margin-bottom: 0px;
  text-align: center;
  margin: 10px auto;
}

ul {
  margin: 0px;
  font-size: 30px;
}

@media screen and (max-width: 975px) {
  ul {
    list-style-type: none;
  }
}
</style>