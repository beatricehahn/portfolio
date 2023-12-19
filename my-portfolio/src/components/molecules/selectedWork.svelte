<script>
    import Work from '../atoms/work.svelte';
</script>

<section id='selected-works-container'>
    <h3>Selected Work</h3>
    <Work />
    <Work />
    <Work />
    <div class='checkout'>
        <a href="/">Check out all work</a>
    </div>
</section>

<style lang='scss'>
    #selected-works-container {
        display: flex;
        flex-direction: column;
        align-items: center;

        margin-top: 64px;
        background-color: rgb(172, 241, 61);
        width: 100%;
        padding-bottom: 64px;

        .checkout {
            padding-top: 16px;
        }
    }
</style>