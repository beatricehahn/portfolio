<script>
    import Work from '../atoms/work.svelte';
</script>

<section id='selected-works-container'>
    <div class='title'>
        <h1>Selected Work</h1>
    </div>
    <ul>
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
        }
    }

    .title {
        text-align: right;

    }

    h1 {
        /* color: $black-900; */
        font-size: clamp(24px, 7vw + 1rem, 72px);
        white-space: nowrap;
        font-family: 'BebasNeue-Regular';
        //padding-right: 16px;
    }

    ul {
        list-style: none;
    }

    a {
        text-decoration: none;
        color: $off-white;
    }

</style>