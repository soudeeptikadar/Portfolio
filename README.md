<!--
**soudeeptikadar/soudeeptikadar** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">
    <title>Portfolio Website</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600&display=swap');

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    text-decoration: none;
    border: none;
    outline: none;
    font-family: 'Poppins', sans-serif;
}

html{
    font-size: 62.5%;
}

body{
    width: 100%;
    height: 100vh;
    overflow-x: hidden;
    background-color: black;
    color: white;
}

header{
    margin-top: 20px;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 1rem 9%;
    background-color: transparent;
    filter: drop-shadow(10px);
    display: flex;
    justify-content: space-between;
    align-items: center;
    z-index: 100;
}

.logo{
    font-size: 3rem;
    color: #b74b4b;
    font-weight: 800;
    cursor: pointer;
    transition: 0.5s ease;
}

.logo:hover{
    transform: scale(1.1);
}

nav a{
    font-size: 1.8rem;
    color: white;
    margin-left: 4rem;
    font-weight: 500;
    transition: 0.3s ease;
    border-bottom: 3px solid transparent;
}

nav a:hover,
nav a.active{
    color: #b74b4b;
    border-bottom: 3px solid #b74b4b;
}

@media(max-width:995px){
    nav{
        position: absolute;
        display: none;
        top: 0;
        right: 0;
        width: 40%;
        border-left: 3px solid #b74b4b;
        border-bottom: 3px solid #b74b4b;
        border-bottom-left-radius: 2rem;
        padding: 1rem solid;
        background-color: #161616;
        border-top: 0.1rem solid rgba(0,0,0,0.1);
    }

    nav.active{
        display: block;
    }

    nav a{
        display: block;
        font-size: 2rem;
        margin: 3rem 0;
    }

    nav a:hover,
    nav a.active{
        padding: 1rem;
        border-radius: 0.5rem;
        border-bottom: 0.5rem solid #b74b4b;
    }
}

section{
    min-height: 100vh;
    padding: 5rem 9% 5rem;
}

.home{
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 8rem;
    background-color: black;
}

.home .home-content h1{
    font-size: 6rem;
    font-weight: 700;
    line-height: 1.3;
}

span{
    color: #b74b4b;
}

.home-content h3{
    font-size: 4rem;
    margin-bottom: 1rem;
    font-weight: 700;
}

.home-content p{
    font-size: 1.6rem;
}

.home-img{
    border-radius: 50%;
}

.home-img img{
    position: relative;
    width: 32vw;
    border-radius: 50%;
    box-shadow: 0 0 25px solid #b74b4b;
    cursor: pointer;
    transition: 0.2s linear;
}

.home-img img:hover{
    font-size: 1.8rem;
    font-weight: 500;
}

.social-icons a{
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 4rem;
    height: 4rem;
    background-color: transparent;
    border: 0.2rem solid #b74b4b;
    font-size: 2rem;
    border-radius: 50%;
    margin: 3rem 1.5rem 3rem 0;
    transition: 0.3s ease;
    color: #b74b4b;
}

.social-icons a:hover{
    color: black;
    transform: scale(1.3) translateY(-5px);
    background-color: #b74b4b;
    box-shadow: 0  0 25px #b74b4b;
}

.btn{
    display: inline-block;
    padding: 1rem 2.8rem;
    background-color: black;
    border-radius: 4rem;
    font-size: 1.6rem;
    color: #b74b4b;
    letter-spacing: 0.3rem;
    font-weight: 600;
    border: 2px solid #b74b4b;
    transition: 0.3s ease;
    cursor: pointer;
}

.btn:hover{
    transform: scale3d(1.03);
    background-color: #b74b4b;
    color: black;
    box-shadow: 0 0 25px #b74b4b;
}

.typing-text{
    font-size: 34px;
    font-weight: 600;
    min-width: 280px;
}

.typing-text span{
    position: relative;
}

.typing-text span::before{
    content: "software Developer";
    color: #b74b4b;
    animation: words 20s infinite;
}

.typing-text span::after{
    content: "";
    background-color: black;
    position: absolute;
    width: calc(100% + 8px);
    height: 100%;
    border-left: 3px solid black;
    right: -8;
    animation: cursor 0.6s infinite;
}

@keyframes cursor{
    to{
        border-left: 3px solid #b74b4b;
    }
}

@keyframes words{
    0%, 20%{
        content: "Web Developer";
    }
    21%, 40%{
        content: "Developer";
    }
    41%, 60%{
        content: "Web Designer";
    }
    61%, 80%{
        content: "Youtuber";
    }
    81%, 100%{
        content: "Script Writer";
    }
}

@media (max-width: 1000px){
    .home{
        gap: 4rem;
    }
}

@media(max-width:995px){
    .home{
        flex-direction: column;
        margin: 5rem 4rem;
    }

    .home .home-content h3{
        font-size: 2.5rem;
    }

    .home-content h1{
        font-size: 5rem;
    }

    .home-img img{
        width: 70vw;
        margin-top: 4rem;
    }
}


    </style>
</head>

<body>
    <header>
        <a href="#" class="logo">Soudeep</a>

        <nav>
            <a href="#" class="active"> Home</a>
            <a href="#">Services</a>
            <a href="#">Skills</a>
            <a href="#">Education</a>
            <a href="#">Experience</a>
            <a href="#">Contact</a>
        </nav>
    </header>
    <section class="home">
        <div class="home-img">
            <img src="main.jpg" alt="">
        </div>
        <div class="home-content">
            <h1>Hi, It's <span>Soudeep Tikadar</span></h1>
            <h3 class="typing-text">I'm a <span></span></h3>
            <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Minus labore dolores esse. Odit similique
                doloribus tenetur doloremque, sunt commodi in ipsa repudiandae debitis deleniti blanditiis quibusdam
                quaerat neque asperiores ea.</p>
            <div class="social-icons">
                <a target="_blank" href="https://www.linkedin.com/in/soudeeptikadar/"><i
                        class="fa-brands fa-linkedin"></i></a>
                <a target="_blank" href="https://github.com/soudeeptikadar"><i class="fa-brands fa-github"></i></a>
                <a target="_blank" href="https://x.com/soudeeptikadar"><i class="fa-brands fa-x-twitter"></i></a>
                <a target="_blank" href="#"><i class="fa-brands fa-instagram"></i></a>
                <a target="_blank" href="https://www.geeksforgeeks.org/user/soudeeptikadar/">GFG</a>
                <a target="_blank" href="https://leetcode.com/u/soudeeptikadar/">
                    <img src="https://upload.wikimedia.org/wikipedia/commons/1/19/LeetCode_logo_black.png"
                        alt="LeetCode" style="width: 20px; height: 20px;">
                </a>
            </div>
            <a href="#" class="btn">Hire me</a>
        </div>
    </section>
</body>

</html>
