<template>
  <nav class="linkList">
    <ul>
        <li v-for="link in links" :key="link.href">
            <Lunk :name="link.href"
            :href="link.href"
            :title="link.title"
            :subtitle="link.subtitle">
            </Lunk>
        </li>

    </ul>
  </nav>
</template>

<script>
    import Lunk from "./Lunk.vue";
    export default {
        props:["links"],
        components:{Lunk}
    }
</script>

<style lang="scss" scoped>
.linkList .link {
  margin: 1vmin 0;
  box-shadow: inset -4px 0 0 0 var(--primary);
  background: var(--light);
  color: var(--dark);
  display: inline-flex;
  padding: 0.5em 0.75em;
}

</style>
