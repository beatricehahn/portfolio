<script>
    import DropdownMenu from '../atoms/menu.svelte';
</script>

<nav>
    <button>logo</button>
    <DropdownMenu />
</nav>

<style lang="scss">
    @import '../../styles/globalVar.scss';

    nav {
        display: flex;
        justify-content: space-between;
        width: calc(100vw - 2 * $container-padding);
        height: 100px;

        button {
            height: 30px;
        }
    }

</style>