<script>
    import DropdownMenu from '../atoms/menu.svelte';
</script>

<nav>
    <a href='/'>
        <img src="/bh-logo-v4.svg" alt="homepage logo">
    </a>
    <DropdownMenu />
</nav>

<style lang="scss">
    @import '../../styles/globalVar.scss';

    nav {
        margin: 1.6 * $container-padding;
        display: flex;
        justify-content: space-between;
        width: calc(100vw - 4 * $container-padding);
        height: 100px;

        img {
            height: 2rem;
        }
    }

</style>