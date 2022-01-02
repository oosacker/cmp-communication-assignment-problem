<template>
  <section>

    <active-user
      :DisplayUser="CaptureUser"
    ></active-user>

    <user-data
      @new-user="captureNewUser"
    ></user-data>

  </section>
</template>

<script>
export default {
  data() {
    return {
      CaptureUser: {
        name: '',
        age: ''
      }
    };
  },
  methods: {
    captureNewUser(nameInput, ageInput) {
      console.log('capture')
      const newUser = {
        name: nameInput,
        age: ageInput
      }
      this.CaptureUser = newUser
      // console.log(this.User)
    }
  },
};
</script>