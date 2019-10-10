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

</div>
</template>
<script>
export default {
  layout: 'SubPages',
   computed: {
      state() {
        return this.name.length >= 4 ? true : false
      },
      invalidFeedback() {
        if (this.name.length > 4) {
          return ''
        } else if (this.name.length > 0) {
          return 'Enter at least 4 characters'
        } else {
          return 'Please enter something'
        }
      },
      validFeedback() {
        return this.state === true ? 'Thank you' : ''
      }
    },
    data() {
      return {
        name: ''
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


