<script>
	import { BtnArrow } from '$lib/index.js';
    import { base } from '$app/paths';

</script>

<section class="heroAbout">
    <div class="heroAboutWrapper">
        <h1>
            ABOUT 
            <span style=" color: var(--Yellow-Primary);">US</span>
        </h1>
        <p> At INK, we're on a mission to transform the lives of young individuals.</p>
        <div class="btnArrow">
            <BtnArrow  href="{base}#introAbout" />
        </div>
    </div>
</section>

<style>

    h1 {
        font-size: 7.5em;
        padding-top: 2em;
    }

    .heroAbout {
        width: 100%;
        height: 50vh;
        display: block;
        text-align: center;
        font-family: var(--Apercu-Font);
    }

    .heroAbout::before {
        content: "";
        background: url(/assets/bg-soccer-field.webp) ;
        background-position: center;
        background-size: cover;
        background-repeat: no-repeat;
        height: clamp(48em, 64vw, 62em);
        opacity: 0.2;
        top: 0;
        left: 0;
        bottom: 0;
        right: 0;
        position: absolute;
        z-index: -1;   
    }

    .heroAboutWrapper {
        position: relative;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -30%);
        display: flex;
        flex-direction: column;
        align-items: center;
        
    }

    .heroAboutWrapper > h1 {
        color: var(--White);
    }

    .heroAboutWrapper > p {
        width: 80%;
        font-size: 2em;
        max-width: 30em;
        padding: 2em;
    }

    .btnArrow {
        display: flex;
        justify-content: center;
    }


    /* 1000px */
    @media (min-width: 62.5em) {

        .heroAbout::before {
            height: clamp(92em, 74vw, 119em);
            background-position-y: -24em;
        }
    }

</style>