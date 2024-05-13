<script>
    import { onMount } from 'svelte';
     
    onMount(() => {
        console.log('attaching particles js');
        const script = document.createElement('script');
        script.src = 'assets/particles.js'; // might be outdated so check for an update can link
        document.body.appendChild(script);

        console.log('attaching app js');
        const config = document.createElement('script');
        config.src = 'assets/app.js'; // might be outdated so check for an update can link
        document.body.appendChild(config);
    });
</script>

<html lang="en">
    <div id="particles-js"></div>
</html>

<style>
    #particles-js {
        width: 100%;
        height: 110%;

        position: absolute;
        top: 120vh;

        background-color: #1c1a1a;
        background-image: url("");
        background-repeat: repeat;
        background-size: cover;
        background-position: 50% 50%;

        z-index: 1;
    }

    @media screen and (min-width: 2000px) {
    #particles-js {
        width: 100%;
        height: 95%;

        position: absolute;
        top: 120vh;

        background-color: #1c1a1a;
        background-image: url("");
        background-repeat: repeat;
        background-size: cover;
        background-position: 50% 50%;

        z-index: 1;
    }
  }
</style>
