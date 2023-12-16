<script>
    import './global.scss';
</script>

<section id='hero-section'>
    <h1>This is the homepage</h1>
    <p id='hero-summary'>This is the hero section text. Lorem Ipsum.
        This is the hero section text. Lorem Ipsum.
        This is the hero section text. Lorem Ipsum.
        This is the hero section text. Lorem Ipsum.
    </p>
</section>

<section id='quote-section'>
    <quote>[Add my quote here later]</quote>
</section>

<section id='about-section'>
    <h2>ABOUT</h2>
    <p>This is description of myself. Placeholder for description.This is description of myself. Placeholder for description. </p>
    <a href='#' class='primary-btn'>Download Resume</a>
</section>

<section id='work-section'>
    <h2>SELECTED WORK</h2>
    <ul>
        <li>
            <div class='project-wrapper'>
                <div class='project-info'>
                    <h6>CATEGORY</h6>
                    <div class='category-divider'></div>
                    <h4>PROJECT TITLE</h4>
                    <p>Short description of what the project is.</p>
                    <a href="#" class='primary-btn'>View Case Study</a>
                </div>
                <div class='project-img-placeholder'>
                    <img src='' alt='project splash screen'>
                </div>
            </div>
        </li>
        
        <li>
            <div class='project-wrapper'>
                <div class='project-info'>
                    <h6>CATEGORY</h6>
                    <div class='category-divider'></div>
                    <h4>PROJECT TITLE</h4>
                    <p>Short description of what the project is.</p>
                    <a href="#" class='primary-btn'>View Case Study</a>
                </div>
                <div class='project-img-placeholder'>
                    <img src='' alt='project splash screen'>
                </div>
            </div>
        </li>
    
        <li>
            <div class='project-wrapper'>
                <div class='project-info'>
                    <h6>CATEGORY</h6>
                    <div class='category-divider'></div>
                    <h4>PROJECT TITLE</h4>
                    <p>Short description of what the project is.</p>
                    <a href="#" class='primary-btn'>View Case Study</a>
                </div>
                <div class='project-img-placeholder'>
                    <img src='' alt='project splash screen'>
                </div>
            </div>
        </li>
    </ul>
</section>

<section id='process-section'>
    <h2>DESIGN AND DEVELOPMENT PROCESS</h2>
    <p>Explanation of my thinking process</p>
    <br>
    <h2>SKILLS</h2>
    <br>
    <h2>TOOLS</h2>
</section>

<section id='contact-section'>
    <h2>CONTACT</h2>
    <div class='email'></div>
    <div class="linkedin"></div>
</section>

<style lang="scss">
    * {
        width: 100vw;
        margin: 0;
    }

    h1, h2, h3, h4, h5, h6 {
        font-family: 'BebasNeue-Regular', sans-serif;
    }

    ul {
        padding: 0
    }

    li {
        list-style-type: none;
    }

    #hero-section {
        height: 90vh;
        background-color: rgb(203, 203, 103);

        h1 {
            font-size: 50px;
        }
        #hero-summary {
            width: 50vw;
        }
    }

    #quote-section {
        background-color: var(--black-800);
        color: var(--off-white);
        height: 10vh;
    }

    #about-section {
        background-color: rgb(216, 129, 129);

        p {
            margin-bottom: 32px;
        }
    }

    #work-section {
        background-color: rgb(33, 155, 155);
    }

    .project-wrapper {
        display: flex;
        padding-top: 64px;
        padding-bottom: 32px;
        .project-info {
            p {
                margin-top: 24px;
                margin-bottom: 24px;
                padding-right: 128px;
            }
        }
    }

    .project-img-placeholder{
        background-color: rgb(186, 134, 235);
        height: 250px;
        width: 400px;
    }

    #process-section {
        background-color: beige;
    }

    #contact-section {
        background-color: var(--black-800);
        color: var(--off-white);
        height: 10vh;
    }
</style>