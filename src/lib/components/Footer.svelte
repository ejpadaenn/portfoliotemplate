<html lang="en">
    <div class="genwrap">
        <h1>'Reach Me'</h1>
        <h2>yournamehere 2024</h2>
        <div class="iconwrapper">
            <a href="http://www.behance.net" target="_blank" rel="noopener noreferrer"><img src="assets/images/socials/bxl-behance.svg" alt="behance" class="icon"/></a>
            <a href="http://www.instagram.com" target="_blank" rel="noopener noreferrer"><img src="assets/images/socials/bxl-instagram.svg" alt="instagram" class="icon"/></a>
            <a href="http://linkedin.com" target="_blank" rel="noopener noreferrer"><img src="assets/images/socials/bxl-linkedin.svg" alt="linkedin" class="icon"></a>
        </div>
    </div>
</html>

<style>
    html {
        height: auto;
        width: auto;
        max-width: 100%;

        background-color: #1c1a1a;
    }

    .genwrap {
        height: 10rem;
        width: 100%;

        background-color: #1c1a1a;
        
        display: grid;
        grid-template-rows: 1fr 1fr;
        grid-template-columns: 0;
        grid-gap: 1rem;
    }

    h1 {
        font-family: "Unbounded", sans-serif;
        font-optical-sizing: auto;
        font-weight: 600;
        font-style: normal;
        color: white;
        font-size: 2rem;

        margin-top: 0;

        grid-area: 1 / 2;
        align-self: start;
        justify-self: center;
    }

    h2 {
        font-family: "Poppins", sans-serif;
        font-optical-sizing: auto;
        font-weight: 300;
        font-style: italic;
        color: white;
        font-size: 1.2rem;

        grid-area: 2 / 2;
        align-self: end;
        justify-self: center;
    }

    .iconwrapper {
        grid-area: 1 / 2;
        align-self: end;
        justify-self: center;
    }

    .icon {
        height: 30px;
        width: 30px;

        filter: invert(100%);

        opacity: 0.4;
    }

    .icon:hover {
        transition: all 0.3s ease-out;
        filter: invert(19%) sepia(76%) saturate(3334%) hue-rotate(354deg) brightness(90%) contrast(93%);
    }
</style>