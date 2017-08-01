<template>
  <div class="hello">
    <h1>Hello {{ name }}!</h1>
    <h1>{{ msg }}</h1>
    <h2>Essential Links</h2>
    <ul>
      <li><a href="https://vuejs.org" target="_blank">Core Docs</a></li>
      <li><a href="https://forum.vuejs.org" target="_blank">Forum</a></li>
      <li><a href="https://gitter.im/vuejs/vue" target="_blank">Gitter Chat</a></li>
      <li><a href="https://twitter.com/vuejs" target="_blank">Twitter</a></li>
      <br>
      <li><a href="http://vuejs-templates.github.io/webpack/" target="_blank">Docs for This Template</a></li>
    </ul>
    <h2>Ecosystem</h2>
    <ul>
      <li><a href="http://router.vuejs.org/" target="_blank">vue-router</a></li>
      <li><a href="http://vuex.vuejs.org/" target="_blank">vuex</a></li>
      <li><a href="http://vue-loader.vuejs.org/" target="_blank">vue-loader</a></li>
      <li><a href="https://github.com/vuejs/awesome-vue" target="_blank">awesome-vue</a></li>
    </ul>
  </div>
</template>

<script>
import axios from 'axios';
import VueGettext from 'vue-gettext'

/****localization*****/
// from ln29 to ln35 having error
// var Vue = require('vue');
// var Lang = require('vuejs-localization');
//
// //specify lang folder, in this case './lang'
// Lang.requireAll(require.context('./lang/', true, /\.js$/));
//
// Vue.use(Lang);

export default {
  name: 'hello',
  data: function(){
    return {
      msg: 'Welcome to Your Vue.js App',
      name: 'Jenny'
    }
  }

  /*****RESTful API call*****/
  // data: () => ({
  //   // return {
  //   //   msg: 'Welcome to Your Vue.js App',
  //   //   name: 'Jenny'
  //   // }
  //   posts:[],
  //   errors: []
  // }),
  //
  // created() {
  //   axios.get(`http://10.128.1.141:9000/api/v1/tms/`)
  //   .then(response => {
  //     // JSON responses are automatically parsed.
  //     this.posts = response.data
  //     console.log(response)
  //     console.log(response.data.objects[0].host)
  //   })
  //   .catch(e => {
  //     this.errors.push(e)
  //   })
  //
  //   // async / await version (created() becomes async created())
  //   //
  //   // try {
  //   //   const response = await axios.get(`http://jsonplaceholder.typicode.com/posts`)
  //   //   this.posts = response.data
  //   // } catch (e) {
  //   //   this.errors.push(e)
  //   // }
  //}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
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
