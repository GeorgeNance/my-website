<template>
    <div class="intro">
            <span class="chirp">hola, hey, hi</span>
            <h1>I'm <strong title="Probably not related to that person you know">George Nance</strong>
                － a designer, developer, and a bucket of problems</h1>
            <p>I'm helping make the web awesome at
                <em>Blueworld</em> and in my freetime I'm doing a lot :
            </p>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>

.intro {
  font-size: 2em;
  margin: 5vmin 0;
}

@media (min-width: 60em) {
  .intro {
    font-size: 3em;
  }
}

.intro strong,
.intro em {
  color: var(--primary);
  cursor: help;
}

.intro strong {
  font-weight: 500;
}

.intro em {
  font-style: normal;
}

.intro s {
  opacity: 0.5;
  white-space: nowrap;
  text-decoration: line-through;
  text-decoration-style: wavy;
  color: var(--primary);
  cursor: help;
}
</style>