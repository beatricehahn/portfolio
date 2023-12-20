<script>
    let isMenuOpen = false;

    // toggles isMenuOpen value
    const handleMenuToggle = () => {
        isMenuOpen = !isMenuOpen;

        if (isMenuOpen) {
            document.getElementById('menu').style.height = '100%';
        }
        else {
            document.getElementById('menu').style.height = '0%';
        }
    }

    // set menu to closed if focus is lost
    // const handleFocusLoss = ({relatedTarget, currentTarget}) => {
    //     if (relatedTarget instanceof HTMLElement && currentTarget.contains(relatedTarget)) return;
    //     isMenuOpen = false;
    // }

    // when user navigates to a different page, close overlay
    const navigate = () => {
        isMenuOpen = false;
        document.getElementById('menu').style.height = '0%';
    }

</script>

<div id='menu' class='overlay'>
    <!-- Overlay content-->
    <ul class='overlay-content'>
        <li><a href="/work" class='menu-link' on:click={navigate}>WORK</a></li>
        <li><a href="/about" class='menu-link'>ABOUT</a></li>
        <li><a href="/workflow" class='menu-link'>SERVICES</a></li>
        <li><a href="/contact" class='menu-link'>CONTACT</a></li>
    </ul>
</div>

<button class='menu-btn' on:click={handleMenuToggle}>MENU</button>

<style lang='scss'>
    @import '../../styles/globalVar.scss';
    @import '../../styles/fonts.css';

    .menu-btn {
        background-color: $ui-btn-grey;
        border-radius: 4px;
        padding-left: 8px;
        padding-right: 8px;
        font-weight: bold;
        height: 32px;
        width: 48px;
        z-index: 20;
    }

    li {
        list-style-type: none;
    }

    .overlay {
        height: 0;
        width: 100%;
        position: fixed;
        z-index: 20;
        left: 0;
        top: 0;
        background-color: rgba(0, 0, 0, 0.9);
        overflow-x: hidden; /* Prevent horizontal scroll */
        transition: 0.5s;
    }

    .overlay-content {
        position: relative;
        top: 25%;
        width: 100%;
        text-align: center;
        margin-top: 30px;
    }

    .menu-link {
        padding: 8px;
        text-decoration: none;
        font-family: 'BebasNeue-Regular';
        font-size: 48px;
        color: $off-white;
        transition: 0.3s;
    }

    .menu-link:hover, .menu-link:focus {
        color: $royal-purple-highlight;
    }

    @media screen and (max-height: 450px) {
        .menu-link {
            font-size: 32px;
        }
    }


</style>