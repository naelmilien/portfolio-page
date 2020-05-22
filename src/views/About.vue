<template>
  <div id="about">
    <div class="profile-pic">
      <img src="../assets/profile-pic.jpeg" alt="picture of me" />
    </div>
    <div class="info">
      <h3>
        Name:
        <span class="answer">Nathanael Milien</span>
      </h3>

      <h3>
        Nickname:
        <span class="answer">Nate</span>
      </h3>
      <h3>
        Home country:
        <span class="answer">Haiti</span>
      </h3>
      <h3>
        Adopted country:
        <span class="answer">USA</span>
      </h3>
      <h3>
        Human languages:
        <span class="answer">French, Haitian Creole, English</span>
      </h3>
      <h3>
        Programming languages:
        <span class="answer">JavaScript, TypeScript, C#, HTML, CSS</span>
      </h3>
      <h3>
        Front-end frameworks:
        <span class="answer">Angular, Vue</span>
      </h3>
      <h3>
        Back-end frameworks:
        <span class="answer">Express.js, .NET Core</span>
      </h3>
      <h3>
        Hobbies:
        <span class="answer">TV, reading, Soccer, and other outdoors activities.</span>
      </h3>
    </div>
  </div>
</template>



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
}

h3 {
  color: #8bf98b;
  font-weight: lighter;
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
