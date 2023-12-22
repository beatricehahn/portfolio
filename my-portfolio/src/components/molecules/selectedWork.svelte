<script>
    import Work from '../atoms/work.svelte';
</script>

<section id='selected-works-container'>
    <h1>Selected Work</h1>
    <ul>
        <li><a href="/work/one"><Work /></a></li>
        <li><a href="/work/two"><Work /></a></li>
        <li><a href="/work/three"><Work /></a></li>
    </ul>
    <div class='checkout'>
        <a href="/work">Check out all work</a>
    </div>
</section>

<style lang='scss'>
    @import '../../styles/globalVar.scss';
    @import '../../styles/fonts.css';

    section {
        padding-top: $page-header-and-footer-margin;
        padding-bottom: $page-header-and-footer-margin;

        color: $off-white;
    }

    h1 {
        /* color: $black-900; */
        font-size: clamp(56px, 7vw + 1rem, 88px);
        white-space: nowrap;
        font-family: 'BebasNeue-Regular';
    }

    ul {
        list-style: none;

        a {
            text-decoration: none;
        }
    }

    #selected-works-container {
        display: flex;
        flex-direction: column;
        align-items: center;

        margin-top: 64px;
        background-color: $black-900;
        width: 100vw;
        

        .checkout {
            padding-top: 16px;
        }
    }
</style>