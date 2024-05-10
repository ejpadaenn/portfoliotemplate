<script>
    console.log("slate3.svelte is loaded!")

    import Footer from '../SlateFooter.svelte'

    import { base } from '$app/paths';
</script>

<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@24,400,0,0" />

<html lang="en">
    <div class="header">
        <h1>'yournamehere'</h1>
        <a href="{base}/" class="backlink"><span class="back material-symbols-outlined">keyboard_backspace</span></a>
    </div>
    <div class="slatelanding">
        <h3>Showcase #3</h3>
        <h2>'Your work title here.'</h2>
    </div>
    <div class="showcase">
        <img src="assets/images/imgdefault.svg" alt="placeholder" class="placeholdimg"/>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam porta lectus nunc, vestibulum venenatis eros imperdiet eu.
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
            <br><br>
            Interdum et malesuada fames ac ante ipsum primis in faucibus. Donec in lectus rutrum, eleifend purus ac, auctor tortor.
            In dapibus quam in nulla sagittis convallis vel ut risus. Ut ac facilisis odio. Integer quis pulvinar neque.
            Vivamus pretium lectus justo, nec pharetra mauris dignissim eu. Cras eu aliquet urna. Vestibulum eu dictum est.
            Proin dignissim, ipsum nec auctor imperdiet, massa justo eleifend lectus, eu ultrices nunc felis vel nibh. Lorem ipsum dolor sit amet, consectetur adipiscing elit.
            Cras sit amet enim turpis. Fusce a ipsum eu dolor finibus posuere a non mauris. Etiam ut eros eu libero interdum ultricies. In vitae diam justo.
            Pellentesque eget mauris porttitor, feugiat est ac, ullamcorper sapien. Phasellus pulvinar tempus sagittis.
            <br><br>
            Maecenas purus nisl, convallis vitae mollis quis, interdum at urna. Sed pharetra vulputate lectus fringilla suscipit.
            Ut malesuada vulputate lacus, eu fringilla augue rhoncus eu. Integer laoreet nibh a nisi faucibus, vitae egestas dolor aliquam.
            Nam a urna ac magna gravida venenatis. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Cras a placerat mi.
            Donec nec vehicula justo. Donec tempor ante sapien, id gravida ex mattis quis.
            <br><br>
            Curabitur dignissim justo vel nisi laoreet, quis pharetra dolor interdum.
            Nunc semper, tellus in pellentesque ornare, purus ligula accumsan tortor, a condimentum velit turpis id eros.
            Praesent eu scelerisque ligula, nec feugiat odio. Nulla facilisi. Aliquam egestas lacinia placerat.
            Suspendisse ac enim suscipit augue vestibulum laoreet sit amet sit amet diam. Ut viverra nulla lorem, a elementum ligula tincidunt non.
            Aenean metus lectus, fermentum non luctus vitae, luctus sed leo. Ut posuere augue metus, vel volutpat orci vehicula et.
            Nunc porta, mauris at venenatis tincidunt, massa ligula iaculis felis, in maximus purus sem id ex.</p>
    </div>

    <Footer />
</html>

<style>
    ::-webkit-scrollbar-button {
        height: 0;
        width: 0;
    }

    ::-webkit-scrollbar-track {
        background-clip: padding-box;
        border: solid transparent;
        border-width: 0 0 0 4px;
    }

    ::-webkit-scrollbar-corner {
        background: transparent;
    }

    html {
        height: auto;
        width: auto;
        max-width: 100%;
        margin: 0;

        background-color: #1c1a1a;
    }

    .header {
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

    .backlink {
        position: absolute;
        right: 5rem;
    }

    .back {
        font-size: 2.5rem;
        color: white;
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

    .slatelanding {
        height: auto;
        width: auto;
        max-width: 100%;

        position: absolute;
        top: 10rem;

        display: flex;
    }

    h2 {
        font-family: "Poppins", sans-serif;
        font-weight: 600;
        font-style: normal;
        color: white;
        font-size: 5rem;

        position: relative;
        left: 1rem;
    }

    h3 {
        font-family: "Poppins", sans-serif;
        font-weight: 300;
        font-style: italic;
        color: white;
        font-size: 1.5rem;

        position: relative;
        left: 11rem;
        top: 1rem;
    }

    .showcase {
        height: 200%;
        width: auto;
        max-width: 100%;

        display: flex;
        flex-wrap: wrap;
        justify-content: center;

        position: relative;
        top: 25rem;
    }

    .placeholdimg {
        height: 40%;
        width: 60%;
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
    }
</style>