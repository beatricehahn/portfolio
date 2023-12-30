<script>
    import Header from '../components/organisms/header.svelte';
    import Footer from '../components/organisms/footer.svelte';
</script>

<!-- <Header /> -->
<main>
    <slot></slot>
</main>
<Footer />

<style lang='scss'>
    @import '../styles/globalVar.scss';
    @import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Roboto&family=Source+Sans+3&display=swap');

    :global(*) {
        margin: 0;
        border: 0;
        padding: 0;
        font-family: 'Source Sans 3', 'Roboto', sans-serif;
    }

    :global(main) {
        display: flex;
        flex-direction: column;
        align-items: center;
        padding-top: $main-padding;
        padding-left: $main-padding;
        padding-right: $main-padding;
    }

</style>