<template>
  <div id="projects">
    <h1 class="project-section-title">Projects</h1>
    <div class="projects">
      <div class="project" v-for="project in projects" v-bind:key="project.alt">
        <img :src="project.src" :alt="project.alt" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  el: "#projects",
  data: () => {
    return {
      projects: [
        {
          src:
            "https://www.ajactraining.org/wp-content/uploads/2019/09/image-placeholder.jpg",
          alt: "project one",
          description: "This is project one"
        },
        {
          src:
            "https://www.ajactraining.org/wp-content/uploads/2019/09/image-placeholder.jpg",
          alt: "project one",
          description: "This is project two"
        },
        {
          src:
            "https://www.ajactraining.org/wp-content/uploads/2019/09/image-placeholder.jpg",
          alt: "project one",
          description: "This is project three"
        },
        {
          src:
            "https://www.ajactraining.org/wp-content/uploads/2019/09/image-placeholder.jpg",
          alt: "project one",
          description: "This is project four"
        },
        {
          src:
            "https://www.ajactraining.org/wp-content/uploads/2019/09/image-placeholder.jpg",
          alt: "project one",
          description: "This is project five"
        },
        {
          src:
            "https://www.ajactraining.org/wp-content/uploads/2019/09/image-placeholder.jpg",
          alt: "project one",
          description: "This is project 6"
        }
      ]
    };
  }
};
</script>

<style scoped>
#projects {
  margin: 50px;
}

#projects .project-section-title {
  text-align: center;
  font-family: "Balsamiq sans", cursive;
  text-decoration: underline;
  color: #8bf98b;
  text-decoration-color: #5e5b5e;
  font-size: 60px;
  font-weight: bolder;
}

.projects {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  flex-wrap: wrap;
}

.project img {
  height: 380px;
  margin-bottom: 50px;
}

@media screen and (max-width: 470px) {
  .projects {
    text-align: center;
  }
  .project img {
    width: 80%;
    height: 80%;
  }
}
</style>