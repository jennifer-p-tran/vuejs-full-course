<script setup>
</script>


<!-- 50:45 Within the template inside of Layout.vue, we need to tell this Layout component
    that it has children contents, and more important we need to speicfy where they
    should be rendered. -->
<template>
    <header>
        <h1 class="text-gradient"> 24H FITNESS </h1>
    </header>
    <main>
        <slot/>
    </main>
    <footer>
        <small>Created by</small>
        <a href="https://github.com/jennifer-p-tran" target="_blank">
            <img alt="pfp" src="https://avatars.githubusercontent.com/u/75240836?v=4"/>
            <p>Jennifer Tran</p>
        </a>
    </footer>
</template>


<style scoped>
    header, footer, main {
        padding: 1rem;
        width: 100%;
        max-width: 600px;
        margin: 0 auto;
    }

    footer {
        display: flex;
        flex-direction: column;
        gap: 0.5rem;
        align-items: center;
        padding: 2rem 0;
        padding-bottom: 3rem;
    }

    footer a {
        display: flex;
        align-items: center;
        gap: 0.5rem;
        padding: 0.3rem;
        padding-right: 0.5rem;
        background: var(--background-muted);
        border-radius: 4rem;
        border: 1px solid transparent;
        transition-duration: 200ms;
        text-decoration: none;
    }

    footer a:hover {
        border-color: var(--color-link);
    }

    footer a img {
        max-width: 30px;
        aspect-ratio: 1/1;
        border-radius: 100%;
    }

</style>