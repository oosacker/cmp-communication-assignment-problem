<template>
  <div>
    <h2>{{ DisplayUser.name }}</h2>
    <h3>{{ DisplayUser.age }}</h3>
  </div>
</template>

<script>
export default {
  data() {
    return {
      
    }
  },
  props: {
    DisplayUser: Object
  }
}
</script>

<style>

</style>