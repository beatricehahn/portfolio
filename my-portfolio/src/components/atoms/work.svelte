<script>
    export let url;
    export let src;
    export let alt;
    export let title;
    export let role;
    export let industry;
</script>

<div class='work-container'>
    <div class="project-info">
        <h6>{title}</h6>
        <p>{role} &#x2022 {industry}</p>
    </div>
</div>

<style lang='scss'>
    @import '../../styles/globalVar.scss';
    @import '../../styles/fonts.css';

    .work-container {
        background-color: rgb(61, 61, 61);
        border-radius: 6px;

        width: calc(100vw - 2 * $main-padding);
        height: calc((100vw - 2 * $main-padding)/2);

        margin-top: $container-padding;
        margin-bottom: $container-padding;

        display: flex;
        align-items: flex-end;

        .project-info {
            color:$off-white;

            h6 {
                font-family: 'Source Sans 3', 'Roboto';
                font-size: clamp(1rem, 2.5vw, 2rem); 
                font-weight: 400;
            }

            p {
                //font-size: clamp(16px, 7vw + 1rem, 18px);
                padding-top: 4px;
                font-size: clamp(.8rem, 2vw, 1.5rem); 
            }

            margin-bottom: 16px;
            margin-left: 16px;
            width: 100%;
        }
    }
</style>

