<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width,
    initial-scale=1.0">
    <title> Personal Portfolio Website HTML CSS Only | Codehal
    </title>
    <link rel="stylesheet" href="style.css">
    <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>

</head>

<body>

    <header class="header">
        <a href="#" class="logo">WELCOME</a>

        <nav class="navbar">
            <a href="#" classe="active ">Home</a>
            <a href="#">About</a>
            <a href="#">Services</a>
            <a href="#">Portfolio</a>
            <a href="#">Contact</a>
        </nav>
    </header>

    <section class="home">
        <div class="home-content">
            <h1>Hi, I'm Yahya Benbaba</h1>
            <h3> Developer</h3>
            <p>As a Transformation Digital student . With a strong background in computer science and web development, I have a deep understanding of the latest technologies and trends in the digital world. My expertise in software development, programming languages, and web technologies allows me to design and develop robust web applications. </p>
            <div class="btn-box">
                <a href="#">Hire Me</a>
                <a href="#">Let's Talk</a>
            </div>
        </div>

        <div class="Home-sci">
            <a href="#"><i class='bx bxl-facebook'></i></a>
            <a href="#"><i class='bx bxl-linkedin' ></i></a>
            <a href="#"><i class='bx bxl-gmail' ></i></a>

        </div>
        
        <span class="Home-imgHover"></span>
    </section>
</body>
  @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800;900&display=swap');
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}

body {
    color: #ededed;
}

.header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 20px 10%;
    background: transparent;
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 100;
}

.logo {
    position: relative;
    font-size: 25px;
    color: #ededed;
    text-decoration: none;
    font-weight: 600;
}
.logo::before{
    content: '';
    position: absolute;
    top: 0;
    right: 0;
    width: 100%;
    height: 100%;
    background:#010d15;
    animation: showRight 1s ease forwards;
    animation-delay: .2s;
    
    
}

.navbar a {
    font-size: 18px;
    color: #ededed;
    text-decoration: none;
    font-weight: 500;
    margin-left: 35px;
    transition: .3s;
}

.navbar a:hover,
.navbar a.active {
    color: #00abf0;
}

.home {
    height: 100vh;
    background: url('home.jpg') no-repeat;
    background-size: cover;
    background-position: center;
    display: flex;
    align-items: center;
    padding: 0 10%;
}

.home-content {
    max-width: 600px;
}

.home-content h1 {
    position: relative;
    font-size: 35px;
    font-weight: 700;
    line-height: 1, 2;
}
.home-content h1::before{
    content: '';
    position: absolute;
    top: 0;
    right: 0;
    width: 100%;
    height: 100%;
    background:#010d15;
    animation: showRight 1s ease forwards;
    animation-delay: .4s;
    
    
}

.home-content h3 {
    position: relative;
    font-size: 32px;
    font-weight: 700;
    color: #00abf0;
}
.home-content h3::before{
    content: '';
    position: absolute;
    top: 0;
    right: 0;
    width: 100%;
    height: 100%;
    background:#010d15;
    animation: showRight 1s ease forwards;
    animation-delay: .8s;
    
    
}

.home-content p {
    position: relative;
    font-size: 16px;
    margin: 20px 0 40px;
}

.home-content p::before{
    content: '';
    position: absolute;
    top: 0;
    right: 0;
    width: 100%;
    height: 100%;
    background:#010d15;
    animation: showRight 1s ease forwards;
    animation-delay: .6.5s;
    
    
}

.home-content .btn-box {
    position: relative;
    display: flex;
    justify-content: space-between;
    width: 345px;
    height: 50px;
}

.home-content .btn-box::before{
    content: '';
    position: absolute;
    top: 0;
    right: 0;
    width: 100%;
    height: 100%;
    background:#010d15;
    animation: showRight 1s ease forwards;
    animation-delay: .6.8s;
    z-index: 2;
    
    
}

.btn-box a {
    position: relative;
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 150px;
    height: 100%;
    background: #00abf0;
    border: 2px solid #00abf0;
    border-radius: 8px;
    font-size: 19px;
    color: #081b29;
    text-decoration: none;
    font-weight: 600;
    letter-spacing: 1px;
    z-index: 1;
    overflow: hidden;
    transition: .5s;
}

.btn-box a:hover {
    color: #00abf0;
}

.btn-box a:nth-child(2) {
    background: transparent;
    color: #00abf0;
}

.btn-box a:nth-child(2):hover {
    color: #081b29;
}

.btn-box a:nth-child(2)::before {
    background: #00abf0;
}

.btn-box a::before {
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 0;
    height: 100%;
    background: #081b29;
    z-index: -1;
    transition: .5s;
}

.btn-box a:hover::before {
    width: 100%;
}

.Home-sci {
    position: absolute;
    bottom: 40px;
    width: 170px;
    display: flex;
    justify-content: space-between;
   
    
}



.Home-sci a {
    position: relative;
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 40px;
    height: 40px;
    background: transparent;
    border: 2px solid #00abf0;
    border-radius: 50%;
    font-size: 20px;
    color: #00abf0;
    text-decoration: none;
    z-index: 1;
    overflow: hidden;
    transition: .5s;
}

.Home-sci a:hover {
    color: #081b29;
}

.Home-sci a::before {
    content: '';
    position: absolute;
    background: #00abf0;
    top: 0;
    left: 0;
    width: 0;
    height: 100%;
    z-index: -1;
    transition: .5s;
}

.Home-sci a:hover::before {
    width: 100%;
}

.Home-imgHover {
    position: absolute;
    top: 0;
    right: 30px;
    width: 500px;
    height: 100%;
    background: transparent;
    transition: 3s;
    animation: manipActiveHover .1s forwards;
    animation-delay: 5s;
    pointer-events: none;
}

.Home-imgHover:hover{
    background: #081b29;
    opacity: .8;
}

.Home-imgHover::after{
    content: '';
    position: absolute;
    top: 0;
    right: 0;
    width: 120%;
    height: 100%;
    background:#010d15;
    animation: showRight 1s ease forwards;
    animation-delay: .5s;
    z-index: 100;
    
    
}
@keyframes showRight {
    100%{
        width: 0;
    }
}
@keyframes  manipActiveHover{
    100% {
        pointer-events: auto;
    }
}
