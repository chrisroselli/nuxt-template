<template>
    <b-navbar toggleable="lg" type="light" variant="light">
          <b-container>
  <b-row>
    <b-col>
      <h3>Footer Title</h3>
      <p>Social currency window of opportunity if you want to motivate these clowns, try less carrot and more stick. What do you feel you would bring to the table if you were hired for this position new economy or globalize.</p>
    </b-col>
    
    <b-col>
  <b-form @submit="onSubmit" @reset="onReset" v-if="show">
      <b-form-group
        id="input-group-1"
        label="Email address:"
        label-for="input-1"
        description="We'll never share your email with anyone else."
      >
        <b-form-input
          id="input-1"
          v-model="form.email"
          type="email"
          required
          placeholder="Enter email"
        ></b-form-input>
      </b-form-group>

      <b-form-group id="input-group-2" label="Your Name:" label-for="input-2">
        <b-form-input
          id="input-2"
          v-model="form.name"
          required
          placeholder="Enter name"
        ></b-form-input>
      </b-form-group>

      <b-form-group id="input-group-3" label="Service:" label-for="input-3">
        <b-form-select
          id="input-3"
          v-model="form.service"
          :options="services"
          required
        ></b-form-select>
      </b-form-group>

      <b-form-group id="input-group-4">
        <b-form-checkbox-group v-model="form.checked" id="checkboxes-4">
          <b-form-checkbox value="me">Check me out</b-form-checkbox>
          <b-form-checkbox value="that">Check that out</b-form-checkbox>
        </b-form-checkbox-group>
      </b-form-group>

      <b-button type="submit" variant="primary">Submit</b-button>
      <b-button type="reset" variant="danger">Reset</b-button>
    </b-form>
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
    data() {
      return {
        form: {
          email: '',
          name: '',
          service: null,
          checked: []
        },
        services: [{ text: 'Select One', value: null }, 'Carrots', 'Beans', 'Tomatoes', 'Corn'],
        show: true
      }
    },
    methods: {
      onSubmit(evt) {
        evt.preventDefault()
        alert(JSON.stringify(this.form))
      },
      onReset(evt) {
        evt.preventDefault()
        // Reset our form values
        this.form.email = ''
        this.form.name = ''
        this.form.service = null
        this.form.checked = []
        // Trick to reset/clear native browser form validation state
        this.show = false
        this.$nextTick(() => {
          this.show = true
        })
      }
    }
  }
</script>
<style>

</style>
