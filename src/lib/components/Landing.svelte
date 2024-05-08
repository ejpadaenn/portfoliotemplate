<script>
    console.log("Landing.svelte is loaded!") //component mount check

    import Carousel from './Carousel.svelte'
</script>

<html lang=en>
    <Carousel duration={2000}/>

    <div id="header">
        <h1>'yournamehere'</h1>
    </div>
</html>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Unbounded:wght@200..900&display=swap');

    @import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&family=Unbounded:wght@200..900&display=swap');

    html {
        background-color: #1c1a1a;
        width: auto;
        max-width: 100%;
        height: 100vh;
        margin: 0;
    }

    html::-webkit-scrollbar {
        display: none;
    }

    #header {
        height: 5rem;
        width: 100vw;
        max-width: 100%;

        background-color: #1c1a1a;
        border-bottom: 2px solid rgba(255 255 255 / 35%);

        position: absolute;
        left: 0px;
        top: 0px;
        z-index: 10;

        display: flex;
        align-items: center;
    }

    h1 {
        font-family: "Unbounded", sans-serif;
        font-optical-sizing: auto;
        font-weight: 500;
        font-style: normal;
        color: white;
        font-size: 1.5rem;
        
        margin-left: 5rem;
    }
</style>