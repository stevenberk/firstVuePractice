<template>
  <div class="hello">
  <div class="holder">
    <ul>
      <li v-for="(data, index) in skills" :key='index'>{{index}}. {{data.skill}}
      </li> 
    </ul>
    <p v-if="skills.length > 1"> You have more than one skill</p>
    <p v-else>You have less than or equal to one skill</p>
  </div>
 </div> 
</template>
 
<script>
export default {
  name: 'practice',
 data() {
   return{
     skills:[
       {"skill" : "vue.js"},
       {"skill" : "Visual studio code"},
       {"skill" : "HTML5"},
       {"skill" : "Vanilla JS"},
       {"skill" : "CSS"},
       {"skill" : "Photoshop"},
       {"skill" : "ms paint"},
       {"skill" : "github"}
     ]
   }
 }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style  scoped>

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
</style>
