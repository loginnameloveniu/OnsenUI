<template>
  <div :is="$options._componentTag.slice(2)">
    <slot></slot>
  </div>
</template>

<script>
  import { deriveEvents, deriveMethods, deriveProperties } from '../mixins/derive';
  export default {
    mixins: [deriveEvents, deriveMethods, deriveProperties]
  };
</script>
