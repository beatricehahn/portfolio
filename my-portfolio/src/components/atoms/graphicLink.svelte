<script>
    export let url;
    export let src;
    export let alt;
</script>

<a href={url} target="_blank" rel="noreferrer">
    <img {src} {alt} />
</a>

<style lang='scss'>
    @import '../../styles/globalVar.scss';

    a {
        img {
            height: 1.6rem;
            width: 1.6rem;
            display: inline;

            &:hover,
            &:focus {
                fill: white;
            }
        }
    }
</style>