<div id='hero-container'>
    <div id="hero-content">
        <div id="hero-header">
            <h1>LARGE TEXT</h1>
            <h1>GOES HERE</h1>
        </div>
        <p id='hero-subtitle'>Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestias id voluptatem voluptatibus minima, dolor, ipsa!</p>
    </div>
</div>

<style lang='scss'>
    @import '../../styles/globalVar.scss';

    #hero-container {
        background-color: rgb(29, 146, 184);
        border-radius: 10px;
        width: calc(100vw - 4 * $header-and-footer-margin);
        height: calc(100vh - 4 * $header-and-footer-margin);
        margin-top: 2*$header-and-footer-margin;
        display: flex;
        align-items: flex-end;

        #hero-content {
            @media screen and (max-width: 800px) {
                display: flex;
                flex-direction: column;
                align-items: center;
            }
            
            padding-left: 2 * $container-padding;
            padding-right: 2 * $container-padding;
            padding-bottom: 3 * $container-padding;
            display: flex;
            flex-direction: row-reverse;
            justify-content: space-between;
            align-items: flex-end;
            width: 100%;

            #hero-header {
                background-color: blue;
                max-width: 50rem;

                h1 {
                    color: $royal-purple-highlight;
                    font-size: clamp(32px, 7vw + 1rem, 80px);
                    white-space: nowrap;
                }
            }

            #hero-subtitle{
                margin-bottom: 24px;
                max-width: 400px;
                padding-top: 32px;
                color: $off-white;
            }
        }


    }
</style>