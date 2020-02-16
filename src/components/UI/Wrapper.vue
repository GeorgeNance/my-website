<template>
    <div class="wrapper">
        <slot></slot>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>
.wrapper {
  margin: auto;
  max-width: 42em;
  padding: 10vmin 2em;
  will-change: transform;
  z-index: 20;
  position: relative;
}
</style>