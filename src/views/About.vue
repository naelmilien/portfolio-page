<template>
  <div id="about">
    <div class="profile-pic">
      <img src="../assets/profile-pic.jpeg" alt="picture of me" />
    </div>
    <ul class="info">
      <li v-for="(value, name) in object" v-bind:key="name">
        {{name}}:
        <span class="answer">{{value}}</span>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  el: "#about",
  data: () => {
    return {
      object: {
        name: "nathanael milien",
        nickname: "nate",
        "home country": "Haiti",
        "adopted country": "USA",
        "human languages": "english, french, haitian creole",
        "programming languages": "JavaScript, TypeScript, C#, HTML, CSS",
        "front-end frameworks": "angular, vue",
        "back-end frameworks": "express.js, .NET Core",
        hobbies: "TV, reading, soccer, hiking, and being outdoors"
      }
    };
  }
};
</script>


<style scoped>
img {
  height: 200px;
  border-radius: 50%;
  position: relative;
  top: 10%;
}

#about {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  font-family: "Anton", sans-serif;
  margin-top: 10%;
  font-size: 18px;
}

ul {
  list-style-type: none;
}

li {
  color: #8bf98b;
  font-weight: lighter;
  text-transform: capitalize;
  padding: 5px;
}

.answer {
  color: #5e5b5e;
}

@media screen and (max-width: 820px) {
  #about {
    flex-direction: column;
    text-align: center;
  }
}
</style>
