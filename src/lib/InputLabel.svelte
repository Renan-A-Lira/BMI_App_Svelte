<script>

export let name;
export let type;
export let v;

function setType(node) {
    node.type = type
}

</script>
<div>
    <label for={name}>{name}</label>
    <input id={name} name={name} bind:value={v} use:setType >
</div>

<style>

    div{
        display: flex;
        font-size: 1.3rem;
    }
    div label {
        flex: 1;
    }

    div input {
        flex: 4;
    }

</style>