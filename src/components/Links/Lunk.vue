<template>
    <a    
    class="link"
    rel="noopener noreferrer"
    target="_blank"
    :href="href"
    title="Opens in a new window">
    <span>{{subtitle}}</span>
    <strong>{{title}}</strong>
    </a>
</template>

<script>
    export default {
        name: 'Lunk',
        props: ["href","title","subtitle"]
    }
</script>

<style lang="scss" scoped>
.link {
  display: flex;
  flex-direction: column;
  transition: 0.25s;
  will-change: transform;
  contain: content;
  color: var(--dark);
  overflow: hidden;
  border-radius: 2px;
}
.link span {
  text-transform: uppercase;
  font-size: 1em;
  letter-spacing: 0.05em;
  font-weight: 400;
  opacity: 0.5;
}

.link strong {
  font-size: 3em;
  font-weight: 900;
  line-height: 0.9;
  margin-left: -0.05em;
  display: flex;
    color: var(--darker);
  justify-content: space-between;
  align-items: baseline;
}

.link strong:after {
  content: "≫";
  font-size: 0.8em;
  margin-left: 1em;
  will-change: transform;
  transform: translateX(0);
  transition: 0.25s;
}

.link:hover,
.link:focus {
  box-shadow: inset -1em 0 1em 0 var(--primary), 0 0.05em 0.5em rgba(0, 0, 0, 0.25);
  border-radius: 2px;
  background: var(--primary);
  transform: scale(1.05);
  z-index: 10;
}

.link:hover strong:after,
.link:focus strong:after {
  transform: translateX(0.125em);
}
</style>