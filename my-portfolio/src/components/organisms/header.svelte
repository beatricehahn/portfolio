<script>
    import Navigation from '../molecules/navigation.svelte';
</script>

<header>
    <Navigation />
</header>

<style lang='scss'>
    @import '../../styles/globalVar.scss';

    header {
        position: fixed;
        top: 0;
        z-index: 100;
        display: flex;
        justify-content: center;
        width: 100vw;
        padding-top: .8 * $container-padding;
    }
</style>