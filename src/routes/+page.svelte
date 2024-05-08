<script>
    console.log("hello world!") //initial script is loaded!

    import Menu from '../lib/components/Menu.svelte'

    import Landing from '../lib/components/Landing.svelte'

    import Portfolio from '../lib/components/Portfolio.svelte'

    import About from '../lib/components/About.svelte'

    import Footer from '../lib/components/Footer.svelte'
</script>

<Menu />

<a id="landingSection">
    <Landing />
</a>

<a id="portfolioSection">
    <Portfolio />
</a>

<a id="aboutSection">
    <About />
</a>

<Footer />