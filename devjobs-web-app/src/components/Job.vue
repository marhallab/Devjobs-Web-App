<template>
  <div class="job">
    <div class="job-logo">
      <img src="//logo.clearbit.com/spotify.com" />
      <p>1h ago full time</p>
    </div>
    <h4>Senior Software Dev</h4>
    <p>Scoot</p>
    <p>USA</p>
  </div>
</template>

<style lang="scss" scoped>
.job {
  width: 300px;
  height: 200px;
  background-color: $white;
  text-align: start;
  padding-left: 30px;

  &-logo {
    display: flex;
    width: 200px;
    justify-content: space-between;
    p {
      margin-top: 10px;
    }

    img {
      width: 50px;
      height: 50px;
    }
  }
}

h4 {
  font-weight: bold;
}

p {
  color: $darkGrey;
}
</style>

<script>
export default {
  props: {
    logo: String,
  },
};
</script>