<script>
    import Work from '../atoms/work.svelte';
</script>

<section id='selected-works-container'>
    <div class='title'>
        <h1>Selected Work</h1>
    </div>
    <ul class='work-wrapper'>
        <li>
            <a href="/work/one">
                <Work 
                    title='Confistand'
                    role='UI/UX'
                    industry='Health Monitoring Web App'
                />
            </a>
        </li>
        <li>
            <a href="/work/two">
                <Work 
                    title='Podcast Blog'
                    role='UI/UX'
                    industry='Entertainment, Education'
                />
            </a>
        </li>
        <li>
            <a href="/work/three">
                <Work 
                    title='Trojan Dining'
                    role='Frontend Development'
                    industry='Food'
                />
            </a>
        </li>
    </ul>
    <div class='checkout'>
        <a href="/work">VIEW ALL PROJECTS</a>
        <img src="/arrow-icon.svg" alt="Arrow">
    </div>
</section>

<style lang='scss'>
    @import '../../styles/globalVar.scss';
    @import '../../styles/fonts.css';
    
    #selected-works-container {
        padding-top: $page-header-and-footer-margin;
        padding-bottom: $page-header-and-footer-margin;
        margin-top: 64px;
        width: 100vw;

        color: $off-white;
        background-color: $black-900;

        display: flex;
        flex-direction: column;
        align-items: center;
    
        .checkout {
            padding-top: 16px;
            display: flex;
            align-items: center;

            a {
                padding-right: 16px;
            }

            img {
                width: 1.2rem;
            }
        }
    }

    .title {
        //text-align: right;
        h1 {
            letter-spacing: 0.5rem;
            font-size: clamp(24px, 7vw + 1rem, 72px);
            white-space: nowrap;
            font-family: 'BebasNeue-Regular';
        }
    }


    .work-wrapper {
        li {
            list-style-type: none;
        }
    }

    a {
        text-decoration: none;
        color: $off-white;
    }

</style>