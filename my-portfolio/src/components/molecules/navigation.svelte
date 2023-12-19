<script>
    import DropdownMenu from '../atoms/menu.svelte';
</script>

<nav>
    <img src="/bh-v2.svg" alt="homepage logo">
    <DropdownMenu />
</nav>

<style lang="scss">
    @import '../../styles/globalVar.scss';

    nav {
        margin: 1.6 * $container-padding;
        display: flex;
        justify-content: space-between;
        width: calc(100vw - 2 * $container-padding);
        height: 100px;

        img {
            height: 48px;
        }
    }

</style>