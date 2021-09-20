<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <JobsList/>
  </div>
</template>

<script>
// @ is an alias to /src
import JobsList from '../components/JobsList.vue'

export default {
  name: 'Home',
  components: {
    JobsList
  }
}
</script>
