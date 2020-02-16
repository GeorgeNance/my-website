<template>

<div>
  <Background></Background>
    <Wrapper>

            <Intro></Intro>
            <LinkList :links="links"></LinkList>

      <Footer></Footer>
    </Wrapper>
    </div>
</template>

<script>
    import Background from '../components/Background/Background';
    import LinkList from '../components/Links/LinkList';
    import Wrapper from '../components/UI/Wrapper';
        import Intro from '../components/Intro';
        import Footer from '../components/Footer';
    export default {
        components: {
            Background,
            LinkList,
            Wrapper,
            Intro,
            Footer
        },
        data() {
            return {
                links: [
                    {
                        href: "https://twitter.com/geonance",
                        title: "Twitter",
                        subtitle: "Lols"
                    },
                    {
                        href: "https://github.com/georgenance",
                        title: "Github",
                        subtitle: "Code"
                    },
                    {
                        href: "https://instagram.com/levelup.mylife",
                        title: "Instagram",
                        subtitle: "Fitness"
                    },
                      {
                        href: "https://dev.to/george",
                        title: "Dev.to",
                        subtitle: "Writing"
                    },
                ]
            }
        },
    }
</script>

<style lang="scss" scoped>

</style>
