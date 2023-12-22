<script>
    let url;
    let src;
    let alt;
</script>

<div class='work-container'>
    <div class="project-info">
        <h6>NAME OF PROJECT</h6>
        <h6>[INDUSTRY]</h6>
    </div>
</div>

<style lang='scss'>
    @import '../../styles/globalVar.scss';
    @import '../../styles/fonts.css';

    .work-container {
        background-color: rgb(61, 61, 61);
        border-radius: 10px;
        width: calc(80vw - 2 * $container-padding);
        height: calc((80vw - 2 * $container-padding)/2);
        margin-top: 2 * $container-padding;
        margin-bottom: 2 * $container-padding;
        display: flex;
        align-items: flex-end;

        .project-info {
            color:$off-white;
            h6 {
                font-family: 'Source Sans 3', 'Roboto';
                font-size: clamp(16px, 7vw + 1rem, 24px);
                font-weight: 400;
            }

            display: flex;
            justify-content: space-between;
            margin-bottom: 20px;
            margin-right: 20px;
            margin-left: 20px;
            width: 100%;
        }
    }
</style>

