<template>
  <div class="hello">
    <h1 v-bind:class="{italics: isItalic}">{{ LaMarseillaise }}</h1>
    <button v-on:click="italicsButton" >Le Button</button>
  </div>
</template>

<script>
export default {
  name: 'FirstPage',
  data(){
    return{
      LaMarseillaise : 'La Marseillaise 🎵',
      devBranch: 'dev'
    }
  },
  methods:{
    italicsButton(){
      this.isItalic ? this.isItalic = false : this.isItalic = true
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.italics{
  font-style: italic;
}
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

      LaMarseillaise : 'La Marseillaise 🎵'