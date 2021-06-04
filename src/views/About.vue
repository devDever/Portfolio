<template>
  <div class="about">
    <div class="container">
      <div class="about_wrapper">
        <div class="about_content">
          <h2>About me</h2>
          <p>
            Hi, I'm Denis – UX/UI designer from Minsk. I'm interested in design
            and everything connected with it. <br />
            I'm studying at courses "Web and mobile design interfaces" in
            IT-Academy. <br />
            Ready to implement excellent projects with wonderful people.
          </p>
        </div>
      </div>
      <div class="skills_wrapper">
        <h2>Skills</h2>
        <div class="skills">
          <ul>
            <li :key="skill" v-for="skill in skills" class="skill">
              <img :src="skill.src" alt="" />
            </li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      skills: [
        { name: "HTML", src: require("../assets/img/html.png") },
        { name: "CSS", src: require("../assets/img/css.png") },
        { name: "JS", src: require("../assets/img/js.png") },
        { name: "git", src: require("../assets/img/git.png") },
        { name: "jquery", src: require("../assets/img/jquery-icon-16.png") },
        { name: "figma", src: require("../assets/img/figma.png") },
        { name: "sass", src: require("../assets/img/sass-logo.png") },
      ],
    };
  },
};
</script>

<style lang="scss">
ul {
  list-style: none;
}
.skills_wrapper {
  .skills {
    ul {
      display: flex;
      img {
        width: 100px;
        height: 100px;
      }
    }
  }
}
.about {
  background-color: #f6f6f6;
  padding-top: 30px;
  text-align: center;
  height: 90vh;
  h2 {
    font-size: 50px;
  }
  .about_content {
    border: 1px solid;
  }
}
</style>
