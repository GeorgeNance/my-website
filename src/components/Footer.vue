<template>
    <footer class="footer">
        <b>Addios!</b>
        
        <p>
            if you want to contact me, send me an <Linky href="mailto:hi@georgenance.com">email</Linky>
            or add me on <Linky  href="https://www.linkedin.com/in/georgenance/">LinkedIn</Linky>
        </p>

        <span> © {{new Date().getFullYear()}} me </span>
        <br>
        <Linky  href="https://github.com/GeorgeNance/my-website">source</Linky>
    </footer>
</template>

<script>
import Linky from "./Links/Linky"
    export default {
        components:{
            Linky
        }
    }
</script>

<style lang="scss" scoped>
    a{
        color: var(--primary);
        text-decoration-color: var(--primary);
        font-weight: 400;
        text-decoration: underline;
    text-decoration-style: solid;
    text-decoration-color: currentcolor;
text-decoration-style: wavy;
    }
    .footer{
  font-size: 1em;
  margin: 5vmin 0;
    }
</style>