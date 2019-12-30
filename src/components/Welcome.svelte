<script>

    export let message = 'Welcome to my component';

    export let image = "";

</script>

<style>

    main{
        position: relative;
        background-position: center;
        background-repeat: no-repeat;
        background-size: cover;
        height: auto;
        display: flex;
        flex-flow: row wrap;
        
    }

    main h3{
        color: #fff;
        margin-top: 3em;
        margin-bottom: 3em;
        position: relative;
        padding: 0.5em;
        border-left: 2px solid white;
        font-style: italic;
    }

    .overlay{
        position: absolute;
        width: 100%;
        height: 100%;
        background-color: rgba(0,0,0,0.6);
    }

    

</style>

<main style="background-image: url({image});">
    <div class="overlay"></div>
    <div class="container">
    
        <div class="row">
            <h3>{message}</h3>
        </div>

    </div>
</main>