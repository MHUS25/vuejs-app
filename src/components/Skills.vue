<template>
  <div class="hello">
    <div class="holder">
      <ul>
        <li v-for="(data, index) in skills" :key='index'>{{ index }}. {{ data.skill }}</li>
      </ul>
      <div v-bind:style="{ backgroundColor: bgColor, width: bgWidth, height: bgHeight }"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Skills',
  data() {
    return {
      skills: [
        {"skill": "JavaScript"},
        {"skill": "Vue.js"}
      ],
      bgColor: 'orange',
      bgWidth: '100%', 
      bgHeight: '30px'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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

.alert {
  background-color: pink;
  width: 100%;
  height: 30px
};
</style>
