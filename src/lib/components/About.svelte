<html lang="en">
    <div id="sectionwrapper1">
        <div class="sectionline"></div>
        <h1>About</h1>
    </div>
    <div class="mainbody">
        <img src="assets/images/imgdefault.svg" alt="placeholder" class="placeholdimg">
        <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam porta lectus nunc, vestibulum venenatis eros imperdiet eu.
            Nulla cursus lectus felis, ac cursus ligula pharetra eget. Etiam malesuada porta tortor at gravida. Vivamus pretium libero vel porta porttitor.
            Ut eu arcu luctus, cursus massa nec, luctus arcu. Sed quam dui, pretium sed vulputate ultricies, accumsan vel lorem.
            Nam non nisi quis arcu mattis placerat ac sit amet mi. Pellentesque quis dolor suscipit, commodo purus at, ornare augue. Pellentesque eu leo turpis.
            Integer sollicitudin a sem eget tempor. Ut sapien turpis, condimentum sed ipsum ac, iaculis convallis neque. Aliquam erat volutpat. Duis non dolor lectus.
            Vestibulum blandit ipsum et aliquet imperdiet. Phasellus eget diam pharetra, tempor urna sed, consequat turpis. Donec ut quam nec augue pulvinar fermentum.
            <br><br>
            Nullam augue massa, malesuada ac eros ac, malesuada commodo sem. Donec ornare metus urna, vel ornare nisi consectetur non. Donec mattis tortor ac hendrerit ornare.
            Integer nec lacus tempor, efficitur libero at, semper velit. Aliquam turpis purus, viverra ac massa et, ultrices lobortis mauris.
            Praesent vulputate enim elit, sit amet egestas lorem faucibus id. Donec consectetur risus id lacinia ultrices. Phasellus cursus magna ut pretium viverra.
            Nulla gravida scelerisque magna, vitae molestie elit luctus id.
        </p>
    </div>
</html>

<style>
    html {
        background-color: #1c1a1a;
        max-width: 100%;
        width: auto;
        height: auto;
        margin-top: 5rem;
    }

    .mainbody {
        width: auto;
        height: auto;
        max-width: 100%;

        display: grid;
        grid-template-rows: 1fr 1fr;
        grid-template-columns: 15% 1fr 15%;
    }

    .placeholdimg {
        height: 500px;
        width: 700px;
        object-fit: cover;

        margin-top: 5rem;
        grid-row: 1;
        grid-column: 2;
        justify-self: center;
    }

    #sectionwrapper1 {
        width: 100%;
        height: auto;
        
        display: grid;
        grid-template-rows: 1fr 1fr;
        grid-template-columns: 10% 1fr 10%;
    }
    
    .sectionline {
        width: 90%;
        height: 2px;
        background-color: rgba(230 50 50 / 35%);

        grid-row: 1 / 2;
        grid-column: 2 / 3;
        align-self: end;
    }

    h1 {
        font-family: "Unbounded", sans-serif;
        font-optical-sizing: auto;
        font-weight: 500;
        font-style: normal;
        color: white;
        font-size: 4rem;

        margin-top: 0;
        grid-row: 2;
        grid-column: 2 / 3;
        align-self: start;
    }

    p {
        height: auto;
        width: 65%;

        font-family: "Poppins", sans-serif;
        font-weight: 400;
        font-style: normal;
        font-size: 1rem;
        color: white;

        margin-top: 5rem;
        text-align: justify;
        text-justify: inter-word;

        grid-row: 2;
        grid-column: 2;
        justify-self: center;
    }
</style>