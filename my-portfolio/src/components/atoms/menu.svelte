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
            <p>CLOSE</p>
    
        {:else}
            <p>MENU</p>
        {/if}
        </button>

        <ul class='dropdown-content' style:visibility={isMenuOpen ? 'visible' : 'hidden'}>
            <li><a href="/work">WORK</a></li>
            <li><a href="/about">ABOUT</a></li>
            <li><a href="/workflow">SERVICES AND WORKFLOW</a></li>
            <li><a href="/contact">CONTACT</a></li>
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

        button {
            background-color: $ui-btn-grey;
            border-radius: 4px;
            padding-left: 8px;
            padding-right: 8px;
            font-weight: bold;
        }

        .dropdown-content {
            position: absolute;
            background-color: orange;
            z-index: 2;
        }
    }

</style>