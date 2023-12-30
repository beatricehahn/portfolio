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
                font-size: clamp(1.2rem, 2.5vw, 2rem); 
                font-weight: 400;
            }

            p {
                font-size: clamp(rem, 2vw, 1.5rem); 
                color: $ui-text-grey;
            }

            margin-bottom: 8px;
            margin-left: 16px;
            width: 100%;
        }
    }
</style>

