<template>
    <b-navbar toggleable="lg" type="light" variant="light">
          <b-container>
  <b-row>
    <b-col>
      <h3>Footer Title</h3>
      <p>Social currency window of opportunity if you want to motivate these clowns, try less carrot and more stick. What do you feel you would bring to the table if you were hired for this position new economy or globalize.</p>
    </b-col>
    
    <b-col>
      <b-form-group
      id="fieldset-1"
      label="Name"
      label-for="input-1"
      :invalid-feedback="invalidFeedback"
      :state="state"
      >
        <b-form-input id="input-1" v-model="name" :state="state" trim></b-form-input>
      </b-form-group>
    </b-col>
    <b-col>
      <b-navbar-nav class="ml-auto">
        <b-nav-item href="#">Link</b-nav-item>
        <b-nav-item href="#">Link</b-nav-item>
        <b-nav-item href="#">Link</b-nav-item>
        <b-nav-item href="#">Link</b-nav-item>
      </b-navbar-nav>
    </b-col>
  </b-row>
  </b-container>
  </b-navbar>
</template>
<script>
  export default {
    computed: {
      state() {
        return this.name.length >= 4 ? true : false
      },
      invalidFeedback() {
        if (this.name.length > 4) {
          return ''
        } 
      }
    },
    data() {
      return {
        name: ''
      }
    }
  }
</script>
<style>

</style>
