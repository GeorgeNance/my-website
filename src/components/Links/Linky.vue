<template>
  <a
    rel="noopener noreferrer"
    target="_blank"
    :href="href"
    title="Opens in a new tab">
    <slot></slot>
  </a>
</template>

<script>
    export default {
        props:["href"]
    }
</script>

<style lang="scss" scoped>

</style>