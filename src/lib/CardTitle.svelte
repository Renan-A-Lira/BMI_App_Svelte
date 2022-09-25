<script>
    export let title;
</script>

<div class="title-card">
    <h3>{title}</h3>
</div>

<style>
    .title-card {
        display: flex;
        justify-content: center;
        
        width: 100%;
        height: 20%;

        background-color: aquamarine;

    }
    .title-card h3 {
        align-self: center;
        font-size: 2rem;
    }
</style>