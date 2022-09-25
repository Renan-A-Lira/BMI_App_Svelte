<script>
    
</script>

<div class="Card">
    <slot>

    </slot>
</div>

<style>
    .Card {
        display: flex;
        flex-direction: column;
        width: 30vw;
        min-width: 400px;
        height: 60vh;

        align-self: center;
        margin: calc((100vh - 60vh) / 2) 0;

        background-color: beige;

        border-radius: 10px;
        overflow: hidden;
    }
    
</style>