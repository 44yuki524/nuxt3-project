<template>
    <header class="header">
        <div class="header_inner">
            <div class="logo">
            <NuxtLink to="/"><img src="../assets/images/Front Line.png" alt="logo"></NuxtLink>
            </div>
            <nav class="header_navi">
                <ul>
                    <li><NuxtLink to="https://port.donnakonishi.com/">Portfolio</NuxtLink></li>
                    <li><NuxtLink to="/message">Message</NuxtLink></li>
                    <li><NuxtLink to="/company">Company</NuxtLink></li>
                </ul>
            </nav>
        </div>
    </header>
    <main>
        <slot />
    </main>
    <footer>
        <nav class="footer_navi">
                <ul>
                    <li><NuxtLink to="https://port.donnakonishi.com/">Portfolio</NuxtLink></li>
                    <li><NuxtLink to="/message">Message</NuxtLink></li>
                    <li><NuxtLink to="/company">Company</NuxtLink></li>
                </ul>
        </nav>
        <p>&copy;Front Line</p>
    </footer>
</template>

<style scoped>
/* header */
    .header {
        width: 100%;
        font-family:Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
        background-color: #fff;
        opacity: 0.7;
        position: fixed;
        top: 0;
        left: 0;
}

    .logo a img {
        width: 200px;
    }

    .header_inner {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 10px 15px;
    }

    .header_navi ul {
        display: flex;
        justify-content: space-between;
    }

    .header_navi ul li {
        list-style: none;
        margin-right: 40px;
    }

    .header_navi ul li a {
        font-size: 1.5rem;
        padding: 5px 0;
        font-weight: bold;
        letter-spacing: .1em;
        color: #555;
        text-decoration: none;
        text-shadow: 1px 2px 3px #808080;
        font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    }

/* footer */
    footer {
        height: auto;
        background-color: #efe44e;
        padding-left: 150px;
        padding-top: 60px;
        padding-bottom: 60px;
    }

    .footer_navi ul {
        display: flex;
        padding: 0;
        margin: 0;
    }

    .footer_navi ul li {
        list-style: none;
        margin-right: 40px;
    }

    .footer_navi ul li a {
        font-size: 1.3rem;
        padding: 5px 0;
        font-weight: bold;
        letter-spacing: .1em;
        color: #fff;
        text-decoration: none;
        font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
    }
    
    footer p {
        font-weight: bold;
        font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
        color:#fff;
        margin: 0;
        margin-top: 20px;
        font-size: 1.0rem;
        letter-spacing: .1em;
    }

    @media screen and (max-width:750px){
    /* header */
        .logo a img {
            width: 100px;
        }
        .header_inner {
            padding: 0px 20px;
        }

        .header_navi ul li {
            margin-right: 10px;
        }

        .header_navi ul li a {
            font-size: 0.7rem;
        }

    /* footer */
        footer {
            padding: 30px 0 25px 0;
            margin: 0;
            text-align: center;
        }

        .footer_navi ul {
            display: block;
            }

        .footer_navi ul li {
            padding: 0;
            margin: 0 0 5px 0;
        }

        .footer_navi ul li a {
            font-size: 1.1rem;
        }

        footer p {
            font-size: 0.9rem;
            margin-top: 20px;
        }
    }
</style>