<template>
  <div id="contacts">
    <h1 class="contact-section-title">Contacts</h1>
    <h1 class="email-message">Email me at nmilien09@gmail.com</h1>
    <h1 class="or">Or...</h1>
    <h1 class="social-media">Catch me on the web by clicking on one of the buttons below</h1>
    <div class="social-media-links">
      <a href="https://github.com/naelmilien" target="_blank" class="github-btn btn">
        <i class="fab fa-github fa-2x"></i>
        <span class="social-button-text">On GitHub</span>
      </a>
      <a
        href="https://www.linkedin.com/in/nathanaelmilien/"
        target="_blank"
        class="linkedin-btn btn"
      >
        <i class="fab fa-linkedin fa-2x" aria-hidden="true"></i>
        <span class="social-button-text">On LinkedIn</span>
      </a>
      <!-- <a href="https://codepen.io/naelmilien/" target="_blank" class="codepen-btn btn">
        <i class="fab fa-codepen fa-2x"></i>
        <span class="social-button-text">On Codepen</span>
      </a>-->
      <a href="https://twitter.com/naelmilien" target="_blank" class="twitter-btn btn">
        <i class="fab fa-twitter fa-2x"></i>
        <span class="social-button-text">On Twitter</span>
      </a>

      <a href="https://twitter.com/naelmilien" target="_blank" class="hackerrank-btn btn">
        <i class="fab fa-hackerrank fa-2x"></i>
        <span class="social-button-text">On Hacckerrank</span>
      </a>
      <!-- <div class="free-code-camp-btn btn">
            <a href="https://www.freecodecamp.com/naelmilien" target="_blank" role="button"
              ><i class="fab fa-free-code-camp fa-2x"><span class="social-button-text">On freeCodeCamp</span></i></a
            >
      </div>-->
    </div>
  </div>
</template>

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

@media screen and (max-width: 560px) {
  #contacts h1 {
    font-size: 25px;
    font-weight: lighter;
  }

  #contacts .contact-section-title {
    visibility: hidden;
  }
}
</style>