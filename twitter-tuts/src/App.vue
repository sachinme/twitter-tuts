<template>
  <div id="app">
    <h1>{{title}}</h1>
    <ul>
      <li v-for="user in users" v-bind:key="user.id">
        {{user.firstname}} {{user.lastname}}
      </li>
    </ul>
  </div>
  
</template>

<script>


export default {
  name: 'App',
  components: {
    
  },
  data(){
    return {
      title:'Welcome to my family',
      followers:0,
      users:[
        {
          id:1,
          username:'sachin_bishwakarma',
          firstname:'Sachin',
          lastname:'Bishwakarma',
          emailid:'sachin.web2@gmail.com',
          isadmin:false
        },
        {
          id:2,
          username:'sansakr_bishwakarma',
          firstname:'Sanskar',
          lastname:'Bishwakarma',
          emailid:'sanskar.web2@gmail.com',
          isadmin:false
        },
        {
          id:3,
          username:'maya_bishwakarma',
          firstname:'Phulmaya',
          lastname:'Bishwakarma',
          emailid:'maya.web2@gmail.com',
          isadmin:false
        },
        {
          id:4,
          username:'sanskriti_bishwakarma',
          firstname:'Sansriti',
          lastname:'Bishwakarma',
          emailid:'sanskriti.web2@gmail.com',
          isadmin:false
        }
      ]

    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
