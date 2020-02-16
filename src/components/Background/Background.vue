<template>
<div class="bg">
<particles></particles>
</div>
  
</template>

<script>
import Particles from "./Particles";
export default {
components: {
  Particles
}
}
</script>

<style lang="scss" scoped>
    .bg{
        position: fixed;

        width: 100%;
   height: 100vh;
        background-color: var(--darker);
  background: linear-gradient(to top left, var(--darker), var(--dark));
  transform: translateZ(-15em) scale(2);
    }
</style>