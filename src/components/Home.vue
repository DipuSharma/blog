<template>
  <h1 class="main">Dipu Main Page</h1>
  <!-- <h1 class="main">Function Result {{ getName() }}</h1>

  <h1 class="main">All Data {{getData("Dipu")}}</h1> -->
  <!-- <button v-on:click="test('Hello dipu')">Click Me</button> -->
  <!-- <button v-on:dblclick="test('Hello dipu Double Click')">Double Click</button> -->
  <!-- <button v-on:click="getData()">Click Me</button>
  <input type="text" v-model="count"/> -->
  <input type="name" placeholder="Enter name" v-model="name"/>
  <br/>
  <br/>
  <input type="email" placeholder="Enter Email" v-model="email"/>
  <br/>
  <br/>
  <input type="password" placeholder="Enter Password" v-model="password"/>
  <br/>  <br/>
  <button type="button" v-on:click="getData()">Submit</button>

</template>

<script>
export default {
  name: 'Home',
  data(){
    return {
      name: null,
      email: null,
      password: null,
    }
  },
  methods: {
    getData(){
      console.log("Form data_________________", this.name, this.email, this.password);
    }
  }
 
}
</script>

<style scoped>
h1 {
  color: blue;
}
</style>