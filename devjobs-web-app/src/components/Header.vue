<template>
  <div class="header">
    <div class="header-content">
      <h1>devjobs</h1>
      <h1>Button</h1>
    </div>
  </div>
</template>

<style  lang="scss" scoped>
.header {
  background-image: url("../assets/desktop/bg-pattern-header.svg");
  background-size: 100% 100%;
  background-repeat: no-repeat;
  width: 100%;
  height: 150px;

  &-content {
    display: flex;
    justify-content: space-between;
    margin-left: 100px;
    margin-right: 100px;
    padding-top: 35px;

        h1{
            color: $white;
        }
  }
}
</style>