<template>
  <div class="jobsList">
    <div v-for="job in jobs" :key="job.id">
      <p>{{ job.title }}</p>
    </div>
  </div>
</template>

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