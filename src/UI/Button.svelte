<script>
    export let disabled = false;
</script>

<button on:click {disabled}>
    <slot />
</button>

<style lang="scss">
    button {
        color: white;
        border: none;
        box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.5);
        border-radius: 5px;
        background: #14637a;
        outline: none;
        padding: 0.5rem;
        cursor: pointer;

        &:hover,
        &:active {
            background: #104f63;
        }

        &:disabled {
            cursor: not-allowed;
            background: lightgray;
            color: darkgray;
        }
    }
</style>
