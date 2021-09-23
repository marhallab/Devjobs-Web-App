<template>
  <div class="home">
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
