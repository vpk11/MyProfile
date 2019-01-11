<template>
  <div class="hello">
    <h1>{{ name }}</h1>
    <h2>{{ designation }}</h2>
    <ul>
      <li v-for="socialLink in socialLinks">
        <a v-bind:href="socialLink.link" target="_blank">
          {{ socialLink.name }}
        </a>
      </li>
    </ul>
    <h3>In Love With</h3>
    <ul>
      <li v-for="language in languages">{{ language.name }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "MainProfile",
  data() {
    return {
      name: "Vishnu Prasad K",
      designation: "Software Engineer",
      socialLinks: [
        { name: "Github", link: "https://github.com/vpk11" },
        { name: "Twitter", link: "https://twitter.com/vpk11" }
      ],
      languages: [
        { name: "Ruby" },
        { name: "JavaScript" },
        { name: "Android Development" }
      ]
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
