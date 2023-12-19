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
        width: calc(100vw - 2 * $container-padding);
        height: calc((100vw - 2 * $container-padding)/1.6) ;
        margin-top: 0.5 * $container-padding;
        margin-bottom: 0.5 * $container-padding;
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

