<script>
    let url;
    let src;
    let alt;
</script>

<div class='work-container'>
    <div class="project-info">
        <h5>Name of Project</h5>
        <h5>[Industry]</h5>
    </div>
</div>

<style lang='scss'>
    @import '../../styles/globalVar.scss';
    .work-container {
        background-color: grey;
        border-radius: 10px;
        width: calc(80vw - 2 * $container-padding);
        height: calc((80vw - 2 * $container-padding)/2);
        margin-top: 2 * $container-padding;
        margin-bottom: 2 * $container-padding;
        display: flex;
        align-items: flex-end;

        .project-info {
            color: white;
            background-color: black;
            display: flex;
            justify-content: space-between;
            margin-bottom: 20px;
            margin-right: 20px;
            margin-left: 20px;
            width: 100%;
        }
    }
</style>

