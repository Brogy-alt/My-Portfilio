<template>
 <div>
        <footer>
            <div class="footer ">
                <div class="row">
                    <ul class="icons">
                        <li><a href="https://www.facebook.com/index.php"><i id="facebook" class="fa fa-facebook text-light"></i></a></li>
                        <li><a href="https://www.instagram.com/?__coig_restricted=1"><i id="ig" class="fa fa-instagram text-light"></i></a></li>
                        <li><a href="https://www.youtube.com/"><i id="yt" class="fa fa-youtube text-light"></i></a></li>
                        <li><a href="https://twitter.com/?lang=en-za"><i id="twitter" class="fa fa-twitter text-light"></i></a></li>
                    </ul>
                </div>

                <div class="row">
                    <ul>
                        <li><a class="text-light" href="#">Contact us</a></li>
                        <li><a class="text-light" href="#">Our Services</a></li>
                        <li><a class="text-light" href="#">Privacy Policy</a></li>
                        <li><a class="text-light" href="#">Terms & Conditions</a></li>
                        <li><a class="text-light" href="#">Career</a></li>
                    </ul>
                </div>

                <div class=" m-0 pb-2 text-light" id="copyright">

                    Copyright © {{ CurrentYear }} - All rights reserved || Designed By: Brogan Gys
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

#facebook:hover{
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
#twitter:hover{
  transform: scale(1.1);
  transition: all ease 500ms;
}

.footer {
    background: #000000;
    padding: 40px 0px;
    font-family: 'Play', sans-serif;
    text-align: center;
   
    
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