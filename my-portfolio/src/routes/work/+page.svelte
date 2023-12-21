<script>
    import Work from '../../components/atoms/work.svelte';
</script>

<section>
    <h1>All Projects</h1>
    
    <ul>
        <li><a href="/work/one"><Work /></a></li>
        <li><a href="/work/two"><Work /></a></li>
        <li><a href="/work/three"><Work /></a></li>
        <li><a href="/work/four"><Work /></a></li>
        <li><a href="/work/five"><Work /></a></li>
    </ul>
</section>

<style lang='scss'>
    @import '../../styles/globalVar.scss';
    @import '../../styles/fonts.css';

    h1 {
        color: $black-900;
        font-size: clamp(56px, 7vw + 1rem, 88px);
        white-space: nowrap;
        font-family: 'BebasNeue-Regular';
    }

    ul {
        list-style: none;
    }
    
    section {
        margin-top: $page-header-and-footer-margin;
        margin-bottom: $page-header-and-footer-margin;
    }
</style>