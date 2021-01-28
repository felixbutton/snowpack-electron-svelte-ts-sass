<article>
    <header>
        <h1>
            <slot name="title" />
        </h1>
    </header>
    <slot />
</article>

<style lang="scss">
    article {
        box-shadow: 2px 1px 2px rgba(0, 0, 0, 0.26);
        color: black;
        background: white;
        border: none;
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 2rem 1rem;
        border-radius: 5px;

        h1 {
            font-weight: lighter;
            font-style: italic;
            margin-top: 0;
        }
    }
</style>
