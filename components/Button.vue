<template>
  <button class="button">
    <div v-if="this.$slots.prefix" class="button-prefix">
      <slot name="prefix" />
    </div>
    <span><slot name="label" /></span>
    <div v-if="this.$slots.suffix" class="button-suffix">
      <slot name="suffix" />
    </div>
  </button>
</template>

<script lang="ts" setup>

</script>

<style lang="scss">
.button {
  display: inline-flex;
  align-items: center;
  
  span {
    font-size: 16px;
    font-weight: 500;
    line-height: 20px;
    color: $purple;
  }

  &-prefix,
  &-suffix {
    display: inline-flex;
    align-items: center;
  }
  &-prefix {
    margin-right: 6px;
  }
  &-suffix {
    margin-left: 6px;
  }
}
</style>