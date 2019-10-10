<template>
  <div>
    <b-img src="https://picsum.photos/1024/400/?image=41" fluid-grow alt="Responsive image"></b-img>
<b-container>
  <b-row>
    <b-col>
      <h1>Contact Us</h1>
      <p>
    To be inspired is to become creative, innovative and energized we want this philosophy to trickle down to all our stakeholders can you ballpark the cost per unit for me offline this discussion and synergize productive mindfulness. Staff engagement quick win we need to future-proof this what about scaling components to a global audience?. Low engagement five-year strategic plan. Turd polishing quick win, yet we need more paper but gain traction, but pre launch churning anomalies three-martini lunch. Anti-pattern run it up the flag pole. Push back great plan! let me diarize this, and we can synchronise ourselves at a later timepoint. It's about managing expectations high performance keywords yet we need to socialize the comms with the wider stakeholder community and touch base, and i’ve been doing some research this morning and we need to better nor pro-sumer software or hammer out.</p>
    </b-col>
  </b-row>
</b-container>
<b-container>
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
</b-container>
</div>
</template>
<script>
export default {
  layout: 'SubPages',
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
<style scoped>
.container {
  margin: 30px auto;
  min-height: 25vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>


