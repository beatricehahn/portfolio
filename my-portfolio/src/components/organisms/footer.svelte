<script>
    import GraphicLink from '../atoms/graphicLink.svelte';
</script>

<footer>
    <ul id='social-icons'>
        <li>
            <GraphicLink src="/github.svg" url="https://github.com/beatricehahn" alt="Github Profile" />
        </li>
        <li>
            <GraphicLink src="/linkedin.svg" url="linkedin.com/in/beatrice-hahn" alt='LinkedIn Profile' />
        </li>
    </ul>
    <p id='email-address'>hahnb@alumni.usc.edu</p>
    <p>California, USA</p>
    <ul id='footer-menu'>
        <li><a href="#about-section">ABOUT</a></li>
        <li><a href="#work-section">WORK</a></li>
        <li><a href="#about-section">RESUME</a></li>
        <li><a href="#contact-section">CONTACT</a></li>
    </ul>
    <span>Beatrice Hahn 2024</span>
    <br/>
    <span>Dev & UI/UX Design &#x2022 Game Design</span>
</footer>

<style lang="scss" scoped>
    @import '../../styles/globalVar.scss';

    footer {
        background-color: $black-800;
        padding: $container-padding;
        color: $off-white;

        #email-address {
            margin-top: 8px;
            margin-bottom: 8px;
        }

        #footer-menu {
            list-style-type: none;
            margin-top: 32px;
            margin-bottom: 32px;

            li > a {
                color: $off-white;
            }
        }

        #social-icons li {
            display: inline;
        } 

        span {
            color: $ui-text-grey;
            font-size: 10px;
        }
    }
</style>