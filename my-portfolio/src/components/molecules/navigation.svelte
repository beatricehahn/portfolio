<script>
    import DropdownMenu from '../atoms/menu.svelte';
</script>

<nav>
    <a href="/"><img src="/logov3.svg" alt="homepage logo"></a>
    <DropdownMenu />
</nav>

<style lang="scss">
    @import '../../styles/globalVar.scss';

    nav {
        margin: 2 * $container-padding;
        display: flex;
        justify-content: space-between;
        width: calc(100vw - 4 * $container-padding);
        height: 100px;

        img {
            height: 32px;
        }
    }

</style>