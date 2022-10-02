<template>
  <div :class="['text', `text--${size}`]">
    <p>
      <slot />
    </p>
  </div>
</template>

<script lang="ts" setup>
withDefaults(
  defineProps<{
    size?: 'small' | 'medium' | 'large',
  }>(),
  {
    size: 'small'
  }
)
</script>

<style lang="scss">
.text {
  display: inline-flex;
  align-items: center;

  p {
    color: $base-white;

    a,strong {
      font-weight: 500;
      color: $purple;
    }
    a {
      text-decoration: underline;
    }
  }
  
  &--small p {
    font-size: 14px;
    line-height: 25px;
  }
  &--medium p {
    font-size: 16px;
    line-height: 29px;
  }
  &--large p {
    font-size: 20px;
    line-height: 36px;
  }
}
</style>