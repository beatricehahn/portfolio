<script>
    let isMenuOpen = false;

    // toggles isMenuOpen value
    const handleMenuToggle = () => {
        isMenuOpen = !isMenuOpen;
    }

    // set menu to closed if focus is lost
    const handleFocusLoss = ({relatedTarget, currentTarget}) => {
        if (relatedTarget instanceof HTMLElement && currentTarget.contains(relatedTarget)) return;
        isMenuOpen = false;
    }
</script>

<div id='menu' on:focusout={handleFocusLoss}>
    <div class='dropdown'>
        <button on:click={handleMenuToggle}>
        {#if isMenuOpen}
            <p>Menu is open!</p>
    
        {:else}
            <p>Menu is closed!</p>
        {/if}
        </button>
        <ul class='dropdown-content' style:visibility={isMenuOpen ? 'visible' : 'hidden'}>
            <li><button>WORK</button></li>
            <li><button>ABOUT</button></li>
            <li><button>SERVICES AND WORKFLOW</button></li>
            <li><button>CONTACT</button></li>
        </ul>
    </div>
</div>

<style lang='scss'>
    @import '../../styles/globalVar.scss';
    
    li {
        list-style-type: none;
    }

    .dropdown {
        float: left;
        overflow: hidden;

        .dropdown-content {

            position: absolute;
            background-color: $off-white;
            z-index: 2;
        }
    }

</style>