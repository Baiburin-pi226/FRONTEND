<script>
    import Router from "svelte-spa-router";
    import routes from "./routes";
</script>

<Router {routes} />

<style>
    :global(*){
        box-sizing: border-box;
    }

    :global(body){
        height: 100vh;
        margin: 0;
    }

    :global(#app){
        min-height: 100%; 
        background: rgba(77,61,255,1);
        background: linear-gradient(0deg, rgba(77,61,255,1) 0%, rgba(0,212,255,1) 100%) no-repeat;

        display: grid;
        grid-template-rows: min-content 1fr;
        align-items: center;
        justify-items: center;
    }

</style>