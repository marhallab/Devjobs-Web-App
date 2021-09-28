<template>
  <div class="switch" @click="changeSwitchValue">
    <div class="switch-wrapper" :class="{ darkMode: value, lightMode: !value }">
      <div class="cicrle"></div>
    </div>
  </div>
</template>

<style lang="scss" scoped>

.switch {
  display: flex;

  &-wrapper {
    height: 22px;
    width: 44px;
    display: flex;
    cursor: pointer;
    border-radius: 22px;
    align-items: center;
    padding: 2px;
    transition: all;
    background: $white;
  }
}

.cicrle {
  background: $violet;
  width: 15px;
  height: 15px;
  border-radius: 15px;
  margin: 1px;
}

.lightMode {
  justify-content: flex-end;
}

.darkMode {
  justify-content: flex-start;
}
</style>

<script>
export default {
  props: ["value"],
  methods: {
    changeSwitchValue() {
      this.$emit("input", !this.value);
      console.log(!this.value);
    },
  },
};
</script>