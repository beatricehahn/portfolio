<script>
    import Header from '../components/organisms/header.svelte';
    import Footer from '../components/organisms/footer.svelte';
</script>

<Header />
<main>
    <slot></slot>
</main>
<Footer />

<style lang='scss'>
    @import '../styles/globalVar.scss';

    :global(*) {
        margin: 0;
        border: 0;
        padding: 0;
        font-family: sans-serif;
    }

    :global(main) {
        display: flex;
        flex-direction: column;
        align-items: center;
        padding-left: $container-padding;
        padding-right: $container-padding;
    }

</style>



<!-- <style lang="scss">
    @import './global.scss';
    li {
        list-style-type: none;
    }
    
    /* NAV SPECIFIC*/
    nav {
        align-items: center;
        background-color: rgba(255, 255, 255, 0.8);
        backdrop-filter: blur(5px);
        display: flex;
        justify-content: space-between;
        position: sticky;
        top: 0;
        z-index: 100;
        
        .nav-links {
            display: flex;
            
            a{
                margin-left: 20px;
                margin-right: 20px;
            }
        }

        .logo-wrapper {
            display: flex;
            align-items: center;
            .logo {
                background-color: var(--black-800);
                height: 20px;
                margin-right: 20px;
                width: 20px;
            }
        }

        .menu-icon {
            border: none;
            img {
                width: 20px;
                height: auto;
            }
        }
    }
    
    
    nav, footer {
        padding-top: 20px;
        padding-left: 16vw;
        padding-right: 16vw;
    }

    /* FOOTER SPECIFIC*/
    footer {
        display: flex;
        justify-content: space-between;
        padding-bottom: 16px;

        span {
            font-size: 10px;
        }
    }

    /* Media query for smaller screens*/
    @media screen and (max-width: 400px) {
        .menu-icon {
            display: block;
        }

        .nav-links {
            .nav-link {
                display: none;
                color: red;
            }
        }

        .show-menu .nav-links {
            display: block;
        }
    }
</style> -->