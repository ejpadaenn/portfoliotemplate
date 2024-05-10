<script>
    import { onMount } from 'svelte';
     
    onMount(() => {
            console.log('attaching particles js');
        const script = document.createElement('script');
        script.src = 'https://cdn.jsdelivr.net/npm/particles.js@2.0.0/particles.min.js'; // might be outdated so check for an update can link
        script.onload = () => {
            console.log('loading particles.js');
            particlesJS.load('particles-js', '/path/to/your/particles.json', () => {
            console.log('particles.js loaded');
         });
       };
       document.body.appendChild(script);
     });
</script>

<html lang="en">
    <div id="particles-js"></div>

    <script src="assets/app.js"></script>
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
</style>