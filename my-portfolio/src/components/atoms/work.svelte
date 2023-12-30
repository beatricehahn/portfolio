<script>
    let url;
    let src;
    let alt;
</script>

<div class='work-container'>
    <div class="project-info">
        <h6>NAME OF PROJECT</h6>
        <p>[Role] &#x2022 [INDUSTRY]</p>
    </div>
</div>

<style lang='scss'>
    @import '../../styles/globalVar.scss';
    @import '../../styles/fonts.css';

    .work-container {
        background-color: rgb(61, 61, 61);
        border-radius: 6px;
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
                font-size: clamp(16px, 7vw + 1rem, 32px);
                font-weight: 400;
            }

            p {
                font-size: clamp(16px, 7vw + 1rem, 18px);
            }

            //display: flex;
            //justify-content: space-between;
            margin-bottom: 20px;
            margin-left: 20px;
            width: 100%;
        }
    }
</style>

