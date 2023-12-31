<script>
    import GraphicLink from '../atoms/graphicLink.svelte';
</script>

<footer>
    <div class='footer-content-wrapper'>
        <div id='contact-info'>
            <h6>Contact Details</h6>
            <div>
                <img src="/email-icon.svg" alt="Email icon">
                <p id='email-address'>hahnb@alumni.usc.edu</p>
            </div>
        </div>
    
        <ul id='social-icons'>
            <h6>Digital Spaces</h6>
            <li>
                <GraphicLink src="/github-icon.svg" url="https://github.com/beatricehahn" alt="Github Profile" />
                <a href="https://github.com/beatricehahn" target="_"><span>Github</span></a>
            </li>
            <li>
                <GraphicLink src="/linkedin-icon.svg" url="https://www.linkedin.com/in/beatrice-hahn/" alt='LinkedIn Profile' />
                <a href="https://www.linkedin.com/in/beatrice-hahn/" target='_'><span>LinkedIn</span></a>
            </li>
            <li>
                <GraphicLink src="/itch-icon.svg" url="https://bardicblaze.itch.io/" alt='Itch.io Profile' />
                <a href="https://bardicblaze.itch.io/" target='_'><span>Itch.io</span></a>
            </li>
        </ul>
    
        <ul id='footer-menu'>
            <h6>Menu</h6>
            <li><a href="#about-section">About</a></li>
            <li><a href="#about-section">Resume</a></li>
            <li><a href="#work-section">Work</a></li>
        </ul>
    </div>

    <div class='copyright-and-other-wrapper'>
        <span class='copyright-and-other'>2023-2024 &copy; Beatrice Hahn</span>
        <span class='copyright-and-other'>Dev & UI/UX Design &#x2022 Game Design</span>
    </div>
</footer>

<style lang="scss" scoped>
    @import '../../styles/globalVar.scss';

    footer {
        background-color: $black-900;
        padding: $main-padding;
        color: $off-white;

        h6 {
            font-size: 1.2rem;
            letter-spacing: 2px;
        }

        .footer-content-wrapper {
            display: flex;
            justify-content: space-around;

            @media  (max-width: 600px) {
                display: flex;
                flex-direction: column;

            }
        }
        
        #contact-info {
            margin-top: 32px;
            margin-bottom: 32px;

            div {
                margin-top: 8px;

                img {
                    margin-left: 4px;
                }
            }

            #email-address {
                padding-left: 16px;
                display: inline;
                color: $ui-text-grey;
            }
        }

        #footer-menu {
            list-style-type: none;
            margin-top: 32px;
            margin-bottom: 32px;

            li {
                margin-top: 16px;
                margin-bottom: 16px;
            }

            li > a {
                color: $ui-text-grey;
                text-decoration: none;
            }
        }

        #social-icons {
            list-style-type: none;
            margin-top: 32px;
            margin-bottom: 32px;

            li {
                padding-bottom: 8px;
                padding-top: 8px;

                display: flex;
                align-items: center;
                
                a {
                    text-decoration: none;
                    color: $ui-text-grey;
                    margin-bottom: 4px;
                }

                span {
                    padding-left: 16px;
                }
            }
        }

        .copyright-and-other-wrapper {
            color: $ui-text-grey;
            font-size: 12px;

            @media screen and (min-width: 601px) {
                /* display: flex;
                align-items: center; */

                .copyright-and-other {
                    padding-right: 8px;
                }

            }

            @media screen and (max-width: 600px) {
                display: flex;
                flex-direction: column;
            }
        }
    }
</style>