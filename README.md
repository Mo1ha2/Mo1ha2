
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="group.css">
    <title>daniel diglah</title>
    <link rel="icon" href="mohamed.jpg">
    <style>
:root{
    --primaryColor:#ff274b;
    --secondaryColor:#f7bcf7;
    --lightColor:#ffffff;
    --bgColor-1:#171a1c;
    --bgColor-2:#22282a;
    --padding:8%;
}

*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

html{
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-size: 16px;
}

.home{
    width: 100%;
    height: 100vh;
    background-color: var(--bgColor-1);
    display: flex;
    flex-direction: column;
}

span{
    color: var(--primaryColor);
}

h2{
    font-size: 2.2rem;
    letter-spacing: 0.12rem;
    cursor: pointer;
    color: var(--lightColor);
}

nav{
    padding-top: 2.8rem;
    padding-left: var(--padding);
    padding-right: var(--padding);
    display: flex;
    justify-content: space-between;
    align-items: center;
}

nav ul li{
    list-style: none;
    display: inline-block;
    margin: 0.8rem 1.5rem;
}

nav ul li a{
    color: var(--lightColor);
    text-decoration: none;
    text-transform: capitalize;
    transition: 0.4s;
}

nav ul li a:hover{
    color: var(--primaryColor);
}

.btn{
    background-color: var(--primaryColor);
    color: var(--lightColor);
    text-decoration: none;
    font-weight: bold;
    padding: 0.81rem 1.87rem;
    border-radius: 30px;
    border: 2px solid transparent;
    transition: 0.4s;
}

.btn:hover{
    background-color: transparent;
    border: 2px solid var(--primaryColor);
}

.content{
    flex-grow: 1;
    padding: var(--padding);
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.container-texts{
    position: relative;
    bottom: 70px;
}

h1{
    font-size: 4.65rem;
    margin: 1.7rem 0;
    color: var(--lightColor);
}

h3{
    font-size: 1.5rem;
    color: var(--lightColor);
    margin-bottom: 3.5rem;
}

h4{
    color: var(--secondaryColor);
    font-size: 1.25rem;
    letter-spacing: 0.12rem;
}

.social{
    margin-top: 3.5rem;
}

.social img{
    margin-right: 2rem;
    width: 2.5rem;
    transition: 0.4s;
}

.social img:hover{
    transform: scale(1.2);
}

.home .container-img{
    width: 45%;
    height: 88%;
    position: relative;
    align-self: flex-end;
}

.container-img img{
    position: absolute;
    bottom: 0%;
    height: 120%;
    transform: translateX(-5%);
    transition: .5s;
}

.container-img img:hover{
    transform: scale(1.1);
}

.about{
    background-color: var(--bgColor-1);
    padding:2rem var(--padding);
    display: flex;
    align-items: center;
    justify-content: space-around;
}

.about .img{
    width: 35%;
}

.gmi{
    background-color: var(--bgColor-2);
    width: 100vh;
}


.about .img img{
    width: 90%;
}

.gmi img{
    width: 35%;
    display: none;
}

.about .text{
    width: 35%;
}

p{
    color: var(--secondaryColor);
    letter-spacing: 1px;
    line-height: 1.5rem;
    font-size: 0.8rem;
}

h5{
    font-size: 1.37rem;
    margin-bottom: 2.5rem;
}

.services{
    background-color: var(--bgColor-1);
    padding:2rem var(--padding);
}

.text-center{
    text-align: center;
}

footer{
    padding: 2rem var(--padding);
    background-color: var(--bgColor-2);
}

footer .footer{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

footer .footer p{
    color: var(--lightColor);
    text-align: center;
    width: 500px;
    margin-top: 1rem;
}

footer .footer .end{
    color: var(--primaryColor);
    margin-top: 1rem;
}

.social a{
    text-decoration: none;
}

button{
    display:none;
    position: relative;
    appearance: none;
    border: none;
    outline: none;
    background-color: none;
    cursor: pointer;
    user-select: none;
}

button img{
    display: block;
    width: 33px;
}










@media screen and (max-width: 575px) {
    :root{
        --padding:1.5rem;
    }
    html{
        font-size: 13px;
    }

    .about{
        display: block;
        text-align: center;
        width: 100%;
        padding: 0;
        margin: 0;
    }
    .about h1{
        font-size: 120%;
        text-align: center;
    }

    button{
        display: block;
    }

    .about .text{
        width: 100%;
    }

    .about .text h5{
        padding: 0;
        text-align: center;
        width: 100%;
    }

    .home .container-img{
        display: none;
    }

    .about{
        padding:2rem var(--padding);
    }

    .gmi{
        width: 100%;
    }
    .gmi img{
        display: block;
        margin:0 31.5%;
    }

    .about .img{
        display:none;
    }
    nav{
        position: fixed;
        top: 0;
        left: 0;
        right: 0;
        height: 82px;
        background-color: var(--bgColor-1);
        border-bottom: 1px solid var(--bgColor-2);
        padding-top: 0;
        z-index: 100;
    }
    nav > a{
        display: none;
    }
    nav ul{
        display: none;
        z-index: 9999999999;
    }

    button::selection ~ nav ul{
        display: block;
        z-index: 9999999999;
    }


    .drop.active nav ul{
        display: block;
    }
    .container-texts{
        bottom: 0;
    }
    .social{
        margin-top: 70px;
    }
    h3{
        margin-top: 40px;
    }
    
}

</style>
</head>
<body>
    <section class="home"id="home" > 
        <nav>
            <h2 >daniel <span>diglah</span></h2>
            <ul id="actions">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About Me</a></li>
                <li><a href="">Discription</a></li>
            </ul>
            <a href="#" class="btn">Subsribe</a>
        </nav>
        <div class="content">
            <div class="container-texts">
                <h4>Hello, my name is</h4>
                <h1>Daniel <span>Diglah</span> </h1>
                <h3>I'm a <span>Back-End</span> Developer.</h3>
                <a class="btn">Dowload Cv</a>
                <div class="social">
                    <a href="https://www.facebook.com/profile.php?id=100075474169199" target="_blank" ><img src="facebook.png" alt=""></a>
                    <a href="instagram.html" target="_blank" ><img src="instagram.png" alt=""></a>
                    <a href="linkedin.html"target="_blank"><img src="linkedin.png" alt=""></a>
                    <a href="http://www.youtube.com/channel/UCJqX5JPvmrdiU4c3EvbY1KA" target="_blank" ><img src="youtube.png" alt=""></a>
                </div>
            </div>
            <div class="container-img">
                <img src="Capture.GIF" alt="">
            </div>
        </div>
    </section>
    <div class="gmi"><img src="about.png" alt=""></div>
    <section class="about" id="about">
        <div class="img"><img src="about.png" alt=""></div>
        <div class="text">
            <h1>About <span>Me</span></h1>
            <h5><span>Back-End</span> Developer</h5>
            <p>
                انا محمد علي, sit amet consectetur adipisicing elit. Accusamus expedita ipsum quisquam beatae eos, tenetur repellendus, iusto exercitationem magni voluptates voluptatibus architecto. Rerum optio impedit facilis quasi obcaecati asperiores eveniet.
            </p>
        </div>
    </section>
    <footer>
        <div class="footer">
            <h2>Daniel <span>Diglah</span></h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Beatae, repellendus?</p>
            <p class="end">Good visit</p>
        </div>
    </footer>
</body>
</html>
