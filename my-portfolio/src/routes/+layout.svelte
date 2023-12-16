<script>
    import './global.scss';
    import MenuIcon from '../public/bh-v2.svg'

    let showMenu = false;

    function toggleMenu() {
        showMenu = !showMenu;
    }
</script>

<nav>
    <div class="logo-wrapper">
        <div class="logo"></div>
        <span>BEATRICE HAHN</span>
    </div>

    <!-- Menu icon viewable for smaller screens -->
    <button tabindex='0' class='menu-icon' on:click={toggleMenu} aria-label='clickable menu button'>
        <img src="{MenuIcon}" alt="Menu Icon">
    </button>

    <!-- Full sized nav links -->
    <ul class='nav-links {showMenu ? 'show-menu' : "" }'>
        <li><a href='#about-section' class='nav-link'>ABOUT</a></li>
        <li><a href='#work-section' class='nav-link'>WORK</a></li>
        <li><a href='#about-section' class='nav-link'>RESUME</a></li>
        <li><a href='#contact-section' class='nav-link'>CONTACT</a></li>
    </ul>
    
</nav>

<main>
    <slot></slot>
</main>

<footer>
    <div id='footer-nav'>
        <ul>
            <span>MENU</span>
            <div class='category-divider'></div>
            <li><a href="#about-section">ABOUT</a></li>
            <li><a href="#work-section">WORK</a></li>
            <li><a href="#about-section">RESUME</a></li>
            <li><a href="#contact-section">CONTACT</a></li>
        </ul>
    </div>
    <div id='footer-contacts'>
        <ul>
            <span>UPDATES</span>
            <div class='category-divider'></div>
            <li><a href="linkedin.com/in/beatrice-hahn">LinkedIn</a></li>
            <li><a href='github'>Github</a></li>
            <li><a href='itch.io'>Itch.io</a></li>
        </ul>
    </div>
    <span>Beatrice Hahn 2024</span>
</footer>

<style lang="scss">
    li {
        list-style-type: none;
    }
    
    /* NAV SPECIFIC*/
    nav {
        align-items: center;
        background-color: rgba(255, 255, 255, 0.8);
        backdrop-filter: blur(5px);
        display: flex;
        justify-content: space-between;
        position: sticky;
        top: 0;
        z-index: 100;
        
        .nav-links {
            display: flex;
            
            a{
                margin-left: 20px;
                margin-right: 20px;
            }
        }

        .logo-wrapper {
            display: flex;
            align-items: center;
            .logo {
                background-color: var(--black-800);
                height: 20px;
                margin-right: 20px;
                width: 20px;
            }
        }

        .menu-icon {
            border: none;
            img {
                width: 20px;
                height: auto;
            }
        }
    }
    
    
    nav, footer {
        padding-top: 20px;
        padding-left: 16vw;
        padding-right: 16vw;
    }

    /* FOOTER SPECIFIC*/
    footer {
        display: flex;
        justify-content: space-between;
        padding-bottom: 16px;

        span {
            font-size: 10px;
        }
    }

    /* Media query for smaller screens*/
    @media screen and (max-width: 400px) {
        .menu-icon {
            display: block;
        }

        .nav-links {
            .nav-link {
                display: none;
                color: red;
            }
        }

        .show-menu .nav-links {
            display: block;
        }
    }
</style>