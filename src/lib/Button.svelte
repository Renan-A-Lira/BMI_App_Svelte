<script>

export let innerText;
export let func;

</script>

<button type="button" on:click={func}>{innerText}</button>

<style>
    button {
        border: none;
        width: 40%;
        height: 2rem;
        align-self: center;

        background-color: #9ac2c2;
    }
    button:active {
        background-color: bisque;
    }
</style>