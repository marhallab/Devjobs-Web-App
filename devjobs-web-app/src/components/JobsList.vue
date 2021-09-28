<template>
  <div class="jobsList">
    <job/>
    <div class="jobsList-jobs" v-for="job in jobs" :key="job.id">
      <p>{{ job.title }}</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>

.jobsList{
 
  &-jobs{
    color: $violet ;
  }
}
</style>

<script>
import gql from "graphql-tag";
import job from "../components/Job.vue"

export default {
  name: "JobsList",
  apollo: {
    jobs: gql`
      query {
        jobs {
          id
          title
        }
      }
    `,
  },
  components:{
    job
  }
};
</script>