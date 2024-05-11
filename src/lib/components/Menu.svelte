<script>
    import { fly } from 'svelte/transition'

    import { backOut } from 'svelte/easing'

    let animate = false

    import { base } from '$app/paths';
</script>

<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@40,300,0,0"/>

<button id="nav-toggle" type="button" on:click={() => (animate = !animate)}>
    <span class="menu-icon material-symbols-outlined">more_horiz</span>
</button>

{#if animate}
    <div id="menu" transition:fly={{
        y: 100,
        easing: backOut
    }}>
        <div id="menu-items">
            <a href="{base}#landingSection" class="menu-item">Home</a>
            <a href="{base}#portfolioSection" class="menu-item">Work</a>
            <a href="{base}#aboutSection" class="menu-item">About</a>
        </div>
    </div>
{/if}

<style>
    @import url('https://fonts.googleapis.com/css2?family=Unbounded:wght@200..900&display=swap');

    @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Unbounded:wght@200..900&display=swap');

    .menu-icon {
        color: white;
        height: 2rem;
        width: auto;

        font-size: 2rem;

        display: block;
        position: absolute;
        left: 50%;
        top: 50%;
        transform: translate(-50%, -50%) scale(0.9);
        opacity: 0;

        transition: transform, opacity;
        transition-timing-function: ease;
        transition-duration: 300ms;

        cursor: pointer;
    }

    #nav-toggle {
        height: 3.5rem;
        width: 3.5rem;

        position: fixed;
        z-index: 10;
        left: 6rem;
        bottom: 6rem;

        background-color: #333333;
        border: 2px solid #e63232;
        border-radius: 3.5rem;

        cursor: pointer;

        transition: transform, background-color;
        transition-timing-function: ease;
        transition-duration: 400ms;
    }

    #nav-toggle:hover {
        opacity: 1;
        transform: scale(1.10);
    }

    #nav-toggle:hover > .menu-icon {
        opacity: 1;
        transform: translate(-50%, -50%) scale(1);
    }

    #nav-toggle:active {
        transform: scale(0.90);
    }

    #menu {
        position: fixed;

        min-width: 10vw;
        max-width: 10vw;
        left: 2rem;
        bottom: 11rem;
        z-index: 5;

        border-radius: 1.5rem;
        border: 2px solid #e63232;

        min-height: 10vw;

        width: auto;
        height: auto;

        display: flex;
        flex-direction: column;
        align-items: center;

        background-color: #333333;

    }
    
    .menu-item {
        color: white;
        font-size: 2rem;
        font-family: "Ibarra Real Nova", serif;

        display: block;
        text-decoration: none;
        padding: 0.5rem;

        z-index: 5;
    }

    #menu-items {
        margin-top: 1rem;
        margin-bottom: 1rem;

        z-index: 5;
    }

    #menu-items:hover > .menu-item {
        opacity: 0.3;
    }

    #menu-items:hover > .menu-item:hover {
        opacity: 1;
    }

    .menu-item {
        font-family: "Poppins", sans-serif;
        font-weight: 500;
        font-style: normal;
        font-size: 1.5rem;

        z-index: 5;
    }
</style>