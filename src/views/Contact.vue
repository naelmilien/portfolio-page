<template>
  <div id="contacts">
    <h1 class="contact-section-title">Contacts</h1>
    <h1 class="email-message">Email me at nmilien09@gmail.com</h1>
    <h1 class="or">Or...</h1>
    <h1 class="social-media">Catch me on the web by clicking on one of the buttons below</h1>
    <div class="social-media-links" v-for="data in socialData" v-bind:key="data.className">
      <a :href="data.src" target="_blank" :class="data.className">
        <i :class="data.icon"></i>
        <span class="social-button-text">On {{data.name}}</span>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  el: "#contact",
  data: () => {
    return {
      socialData: [
        {
          name: "GitHub",
          icon: "fab fa-github fa-2x",
          src: "https://github.com/naelmilien",
          className: "github-btn btn"
        },
        {
          name: "LinkedIn",
          icon: "fab fa-linkedin fa-2x",
          src: "https://www.linkedin.com/in/nathanaelmilien/",
          className: "linkedin-btn btn"
        },
        {
          name: "Twitter",
          icon: "fab fa-twitter fa-2x",
          src: "https://twitter.com/naelmilien",
          className: "twitter-btn btn"
        },
        {
          name: "Hackerrank",
          icon: "fab fa-hackerrank fa-2x",
          src: "https://www.hackerrank.com/naelmilien",
          className: "hackerrank-btn btn"
        }
        // {
        //   name: "freeCodecamp",
        //   icon: "fab fa-free-code-camp fa-2x",
        //   src: "https://www.freecodecamp.org/naelmilien",
        //   className: "freecodecamp-btn btn"
        // },
        // {
        //   name: "Codepen",
        //   icon: "fab fa-codepen fa-2x",
        //   src: "https://codepen.io/naelmilien",
        //   className: "codepen-btn btn"
        // }
      ]
    };
  }
};
</script>

<style scoped>
#contacts .contact-section-title {
  font-size: 60px;
  font-family: "Balsamiq sans", cursive;
  text-decoration: underline;
  color: #8bf98b;
  text-decoration-color: #5e5b5e;
}

#contacts h1 {
  font-family: "Anton", sans-serif;
  text-align: center;
  font-size: 30px;
}

#contacts {
  font-family: "Anton", sans-serif;
  margin-bottom: 50px;
}

.btn {
  display: block;
  width: 400px;
  height: 50px;
  border-radius: 5px;
  text-align: center;
  font-family: "Anton";
  margin: 10px auto;
}

a {
  text-decoration: none;
}

.github-btn {
  background-color: #24292e;
}

.linkedin-btn {
  background-color: #3b77b5;
}

.twitter-btn {
  background-color: #60b5f0;
}

.free-code-camp-btn {
  background-color: #2d6502;
}

.codepen-btn {
  background-color: #000000;
}

.hackerrank-btn {
  background-color: #61c967;
}

i {
  color: white;
  display: inline-block;
  padding-top: 10px;
  vertical-align: middle;
}

.social-button-text {
  font-size: 12px;
  color: white;
  padding-left: 12px;
  font-family: Arial, Helvetica, sans-serif;
  margin-top: 80px;
  align-self: end;
}

.email-message,
.social-media {
  color: #8bf98b;
}

.social-media-links {
  margin: 5px;
}

@media screen and (max-width: 560px) {
  #contacts h1 {
    font-size: 25px;
    font-weight: lighter;
  }

  #contacts .contact-section-title {
    visibility: hidden;
  }

  .btn {
    width: 80%;
  }
}
</style>