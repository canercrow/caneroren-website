<template>
  <section class="app">
    <NuxtLoadingIndicator color="#6B6BDE" />
    <div class="container">
      <ProfilePicture />
      <div class="app-inner">
        <Nav />
        <NuxtPage />
      </div>
    </div>
  </section>
</template>

<script lang="ts" setup>

</script>

<style lang="scss">
.app {
  display: flex;
  align-items: flex-start;
  min-height: 100vh;
  padding: 104px 0;

  .container {
    display: flex;
    align-items: flex-start;
  }

  &-inner {
    padding-top: 30px;
  }
}
</style>