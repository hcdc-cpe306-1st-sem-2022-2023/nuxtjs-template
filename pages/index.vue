<template>
  <div>
    <h1>{{ `${firstName} ${lastName}` }}</h1>

    <v-btn> Primary </v-btn>
  </div>
</template>

<script>
export default {
  data() {
    return {
      firstName: 'John',
      lastName: 'Doe',
    }
  },
  // beforeCreate() {
  //   console.log('beforeCreate is called')
  // },
  // beforeMount() {
  //   console.log('beforeMounted is called')
  // },
  mounted() {
    console.log('mounted is called')
  },
  beforeDestroy() {
    console.log('beforeDestroy is called')
    alert('Why leave me?')
  },
}
</script>

<style scoped>
.error {
  color: blue;
}
</style>
