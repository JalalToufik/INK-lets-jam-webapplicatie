<script>
	import { BtnArrowBlue } from '$lib/index.js';
    import { base } from '$app/paths';
</script>

<section class="heroPromise">
    <div class="heroPromiseWrapper">
        <h1>
            Our 
            <span style=" color: var(--Blue-Secondary);">promise</span>
        </h1>
        <p>
            We strive to create a level playing field for all, and we work to 
            ensure that everyone has the opportunity to succeed.
        </p>
        <div class="btnArrow">
            <BtnArrowBlue href="{base}/promise/#introPromise" />
        </div>
    </div>
</section>

<style>
    .heroPromise {
        width: 100%;
        height: 70vh;
        display: block;
        text-align: center;
    }

    /* Background image */
    .heroPromise::before {
        content: "";
        background: url(/assets/PromiseHeroImg800x1200.webp);
        background-position: center;
        background-size: cover;
        opacity: 0.2;
        top: 0;
        left: 0;
        bottom: 0;
        right: 0;
        position: absolute;
        z-index: -1;   
    }

    .heroPromiseWrapper {
        position: relative;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -30%);
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .heroPromiseWrapper > h1 {
        color: var(--White);
        font-size: 7.5em;
        text-transform: uppercase;
    }

    .heroPromiseWrapper > p {
        width: 30em;
        font-family: var(--Apercu-Font);
        font-size: 2em;
        padding: 1em;
    }

    .btnArrow {
        display: flex;
        justify-content: center;
    }

        @media (min-width: 560px) { 
            .heroPromise::before {
                background: url(/assets/PromiseHeroImg560x1200.webp);
            }
    }

        @media (min-width: 640px) { 
            .heroPromise::before {
                background: url(/assets/PromiseHeroImg1920x1080.webp);
                background-position: center;
        }
    }

</style>