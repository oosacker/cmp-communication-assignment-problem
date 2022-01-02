<template>
  <div>
    <form @submit.prevent="submitBtnClick()">
      <input type="text" v-model="NameInput">
      <input type="text" v-model="AgeInput">
      <button type="submit">SUBMIT</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      NameInput: '',
      AgeInput: ''
      
    }
  },
  methods: {
    submitBtnClick() {
      // console.log(`${this.User.Name} ${this.User.Age}`)
      console.log('emit')
      this.$emit('new-user', this.NameInput, this.AgeInput)
    }
  }
}
</script>

<style>

</style>