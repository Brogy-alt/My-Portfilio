<template>
 <div class="">
        <footer class="position-relative">
            <div class="footer">
                <div class="row">
                    <ul class="icons">
                        <li><a href="https://www.linkedin.com/in/brogan-gys/"><i id="linkedin" class="fa fa-linkedin text-light"></i></a></li>
                        <li><a href="https://www.instagram.com/prodbrogy/"><i id="ig" class="fa fa-instagram text-light"></i></a></li>
                        <li><a href="https://www.youtube.com/channel/UC13tr7mMjdQfZRaoI0rbTgQ"><i id="yt" class="fa fa-youtube text-light"></i></a></li>
                        <li><a href="https://github.com/Brogy-alt"><i id="github" class="fa-brands fa-github text-light"></i></a></li>
                    </ul>
                </div>

                <div style="padding-bottom: 1rem; padding-top: 1rem;">
                   <h5 >QUICK LINKS</h5> 
                </div>
                <div class="row" style="font-size: smaller;">
                    
                    <ul>
                        <li><a class="home text-light" href="/">HOME</a></li>
                        <li><a class="about text-light" href="/about">ABOUT</a></li>
                        <li><a class="resume text-light" href="/resume">RESUME</a></li>
                        <li><a class="skills text-light" href="/skills">SKILLS</a></li>
                        <li><a class="contactme text-light" href="/contact">CONTACT ME</a></li>
                    </ul>
                </div>

                <div class=" m-0 pb-2 text-light" id="copyright">

                    <p>Copyright © {{ CurrentYear }} - All rights reserved || Designed By: Brogan Gys</p>
                </div>
            </div>
        </footer>
    </div>
</template>
<script>
export default {
    data(){
        return {
            CurrentYear: new Date().getFullYear()
        }
    }
}
</script>

<style scoped>

p,h2,h3,h3,h4,h5{
  font-family: 'Fjalla One', sans-serif;
}

#linkedin:hover{
  transform: scale(1.1);
  transition: all ease 500ms;
}
#ig:hover{
  transform: scale(1.1);
  transition: all ease 500ms;
}
#yt:hover{
  transform: scale(1.1);
  transition: all ease 500ms;
}
#github:hover{
  transform: scale(1.1);
  transition: all ease 500ms;
}



.footer {
    background: #000000;
    padding: 40px 0px;
    font-family: 'Play', sans-serif;
    text-align: center;
    background: linear-gradient(rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 1)),
    

}
.footer #copyright {
    width: 100%;
    margin: 0px 10px;
    padding: 0.6% 0%;
    color: rgb(0, 0, 0);
    font-size: 1rem;
}
.footer .row a {
    text-decoration: none;
    color: rgb(0, 0, 0);
    transition: 0.5s;
}
.footer .row a:hover {
    color: #0800007a;
}
.footer .row ul {
    width: 100%;
}
.footer .row ul li {
    display: inline-block;
    margin: 0px 30px;
}
.footer .row a i {
    font-size: 2em;
    margin: 0% 1%;
}
@media (max-width:300px) {
    .footer {
        text-align: left;
        padding: 5%;
    }
    .footer .row ul li {
        display: block;
        margin: 10px 0px;
        text-align: left;
    }
    .footer .row a i {
        margin: 0% 3%;
    }
}
@media(max-width: 300px) {
    .footer .row .icons{
        gap: 40px;
        display: flex;
    }
}
</style>  