<template>
  <div class="jobsList">
    <div class="jobsList-jobs" v-for="job in jobs" :key="job.id">
      <p>{{ job.title }}</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>

.jobsList{
  background-color: red;

  &-jobs{
    color: $violet ;
  }
}
</style>

<script>
import gql from "graphql-tag";

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
};
</script>