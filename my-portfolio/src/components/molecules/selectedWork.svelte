<script>
    import Work from '../atoms/work.svelte';
</script>

<section id='selected-works-container'>
    <div class='title'>
        <h1>Selected Work</h1>
    </div>
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
    
    #selected-works-container {
        padding-top: $page-header-and-footer-margin;
        padding-bottom: $page-header-and-footer-margin;
        /* padding-left: 16px;
        padding-right: 16px; */
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
        //width: 100vw;
    }

    h1 {
        /* color: $black-900; */
        font-size: clamp(24px, 7vw + 1rem, 88px);
        white-space: nowrap;
        font-family: 'BebasNeue-Regular';
        //padding-right: 16px;
    }

    ul {
        list-style: none;

        a {
            text-decoration: none;
        }
    }

</style>