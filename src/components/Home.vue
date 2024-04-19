<template>
    <div>
      <h1>Simple Form</h1>
      <p>{{ form }}</p>
      <form>
        <label>Email :</label>
        <input type="email" placeholder="Enter email" v-model="form.email"><br><br>
        <label>Password :</label>
        <input type="password" placeholder="Enter password" v-model="form.password"><br><br>
        <label>Country :</label>
        <select v-model="form.country">
          <option value="" disabled selected>Please select a country</option>
          <option value="India">India</option>
          <option value="China">China</option>
          <option value="USA">USA</option>
        </select><br><br>

        <h3>Techonology</h3>
        <label>Java :</label>
        <input type="checkbox" value="java" v-model="form.technology"><br><br>
        <label>.Net :</label>
        <input type="checkbox" value=".net" v-model="form.technology"><br><br>

        <h3>Techonology</h3>
        <label>Male :</label>
        <input type="radio" value="male" name="gender" v-model="form.gender"><br><br>
        <label>Fimale :</label>
        <input type="radio" value="female" name="gender" v-model="form.gender"><br><br>

        <button type="button" @click="login">Login</button>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    name: 'HomE',
    data() {
      return {
        form: {
            email: '',
            password: '',
            country: '',
            technology : [],
            gender : ''
        }
      }
    },
    methods: {
      login() {
        console.warn("Login data", this.form);
      }
    }
  };
  </script>
  
  <style scoped>
  h1 {
    color: orange;
  }
  </style>
  