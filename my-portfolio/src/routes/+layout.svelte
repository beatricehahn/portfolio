<script>
    import './global.css';
</script>

<nav>
    <div class="logo-wrapper">
        <div class="logo"></div>
        <span>BEATRICE HAHN</span>
    </div>
    <div>
        <ul class='nav-links'>
            <li><a href='#about-section' class='nav-link'>ABOUT</a></li>
            <li><a href='#work-section' class='nav-link'>WORK</a></li>
            <li><a href='#about-section' class='nav-link'>RESUME</a></li>
            <li><a href='#contact-section' class='nav-link'>CONTACT</a></li>
        </ul>
    </div>
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

<style>
    nav {
        align-items: center;
        background-color: rgba(255, 255, 255, 0.8);
        backdrop-filter: blur(5px);
        display: flex;
        justify-content: space-between;
        position: sticky;
        top: 0;
        z-index: 100;
    }

    .nav-links {
        display: flex;
    }

    .nav-links > li > a {
        margin-left: 20px;
        margin-right: 20px;
    }
    .logo-wrapper {
        display: flex;
        align-items: center;

    }
    .logo {
        background-color: var(--black-800);
        height: 20px;
        margin-right: 20px;
        width: 20px;
    }

    li {
        list-style-type: none;
    }

    nav, footer {
        padding-top: 5vh;
        padding-left: 96px;
        padding-right: 96px;
    }

    footer {
        display: flex;
        justify-content: space-between;
        padding-bottom: 16px;
    }

    footer > span {
        font-size: 10px;
    }
</style>