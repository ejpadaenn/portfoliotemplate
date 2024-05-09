<script>
    console.log("Portfolio.svelte is loaded!")

    import { base } from '$app/paths';
</script>

<html lang=en>
    <div id="sectionwrapper1">
        <div class="sectionline"></div>
        <h1>My Work</h1>
    </div>

    <div class="cardwrapper">
        <div class="card">
            <div class="cardtext">Blank Slate</div>
            <!-- svelte-ignore a11y-missing-content -->
            <a href="{base}/blankslate1" class="cardlink"></a>
        </div>
        <div class="card">
            <div class="cardtext">Blank Slate</div>
            <!-- svelte-ignore a11y-missing-content -->
            <a href="{base}/blankslate2" class="cardlink"></a>
        </div>
        <div class="card">
            <div class="cardtext">Blank Slate</div>
            <!-- svelte-ignore a11y-missing-content -->
            <a href="{base}/blankslate3" class="cardlink"></a>
        </div>
        <div class="card">
            <div class="cardtext">Blank Slate</div>
            <!-- svelte-ignore a11y-missing-content -->
            <a href="{base}/blankslate4" class="cardlink"></a>
        </div>
        <div class="card">
            <div class="cardtext">Blank Slate</div>
            <!-- svelte-ignore a11y-missing-content -->
            <a href="{base}/blankslate5" class="cardlink"></a>
        </div>
        <div class="card">
            <div class="cardtext">Blank Slate</div>
            <!-- svelte-ignore a11y-missing-content -->
            <a href="{base}/blankslate6" class="cardlink"></a>
        </div>
    </div>
    <div id="particles-js"></div>

    <script src="assets/particles.js"></script>
    <script src="assets/app.js"></script>

</html>

<style>
    html {
        background-color: #1c1a1a;
        max-width: 100%;
        height: auto;
        margin: 0;
    }

    html::-webkit-scrollbar {
        display: none;
    }

    .card {
        height: 25rem;
        width: 25rem;
        background-color: #444444;

        cursor: pointer;

        display: flex;
        align-items: center;
        justify-content: center;

        position: relative;

        z-index: 2;
    }

    .cardlink {
        content: "";
        position: absolute;
        top: 0px;
        right: 0px;
        bottom: 0px;
        left: 0px;
    }

    .cardtext {
        font-family: "Poppins", sans-serif;
        font-weight: 200;
        font-style: normal;
        font-size: 1rem;
        color: white;

        z-index: 5;
        opacity: 0;
    }

    .card:hover {
        transition: all 0.5s ease-out;
        filter: brightness(70%);
    }

    .card:hover .cardtext {
        transition: all 0.3s ease-out;
        opacity: 100;
    }

    .cardwrapper {
        height: auto;

        display: flex;
        justify-content: center;
        flex-wrap: wrap;

        gap: 3rem;
        padding: 5rem;
    }

    #particles-js {
        width: 100%;
        height: 120%;

        position: absolute;
        top: 120vh;

        z-index: 1;
    }

    #sectionwrapper1 {
        width: 100%;
        height: auto;
        
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
    }
    
    .sectionline {
        width: 90%;
        height: 2px;
        background-color: white;

        margin-top: 2rem;
    }
    
    h1 {
        font-family: "Unbounded", sans-serif;
        font-optical-sizing: auto;
        font-weight: 500;
        font-style: normal;
        color: white;
        font-size: 3rem;

        margin-bottom: 0;
    }
</style>