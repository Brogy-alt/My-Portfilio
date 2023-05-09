<template>
    <div class="skills-page">
      <main>
        <section id="skills-page">
          <div class="container-fluid ">
            <NavbarC/>
            <div class="row d-flex flex-column flex-md-row">
              <div loading="lazy" class="img1 img-fluid">
                <div class="home-text col">
                  <h1 
                    id="heading-skillspage"
                    style="padding-top: 15rem; font-size: 50px"
                    class="lead display-6">
                    SKILLS AND PROJECTS
                  </h1>
                </div>
              </div>
            </div>
          </div>
        </section>
      </main>

      <div class="skills-section">
    <div class="skills-header">
     <h2 class="skills-heading text-dark">SKILLS</h2>   
     </div>
     <div class="skills-container">
       
      <div class="skills-box">
       <div class="skills-title">
       <div class="skills-img">
        <img src="https://i.postimg.cc/vB9bnM6B/html-img.png" alt="" class="skills-icons">
        
        </div>
         <h3>HTML 5</h3>
        </div>
   
       </div>
       
       
        <div class="skills-box">
       <div class="skills-title">
       <div class="skills-img">
        <img src="https://i.postimg.cc/QMG6t3sS/css-icon.png" alt="" class="skills-icons">
        
        </div>
        <h3>CSS3</h3>
        </div>
     
       </div>
       
       
        <div class="skills-box">
       <div class="skills-title">
       <div class="skills-img">
        <img src="https://i.postimg.cc/MGpDPb02/javascript-icon.png" alt="" class="skills-icons">
        </div>
        <h3>JAVASCRIPT</h3>
        </div>
       
       </div>
       
          <div class="skills-box">
       <div class="skills-title">
       <div class="skills-img">
        <img src="https://i.postimg.cc/xTQLp3Yx/nodejs-icon.png"  alt="" class="skills-icons">
        </div>
        <h3>NODE.JS</h3>
        </div>
     
       </div>
       
          <div class="skills-box">
       <div class="skills-title">
       <div class="skills-img">
        <img src="https://i.postimg.cc/BnBgqwZ1/mysql-icon.png" alt="" class="skills-icons">
        </div>
        <h3>MSQL</h3>
        </div>
    
       </div>

       <div class="skills-box">
       <div class="skills-title">
       <div class="skills-img">
        <img src="https://i.postimg.cc/g2gSWkKZ/icons8-bootstrap-512.png" alt="" class="skills-icons">
        </div>
        <h3>BOOSTRAP</h3>
        </div>
    
       </div>

       <div class="skills-box">
       <div class="skills-title">
       <div class="skills-img">
        <img src="https://i.postimg.cc/P5dDMWYW/Ui-ux-icon.png" alt="" class="skills-icons">
        </div>
        <h3>UI/UX</h3>
        </div>
    
       </div>

       
       <div class="skills-box">
       <div class="skills-title">
       <div class="skills-img">
        <img src="https://i.postimg.cc/V604cq7S/wordpress-icon.png" alt="" class="skills-icons">
        </div>
        <h3>WORDPRESS</h3>
        </div>
    
       </div>

      
       
          <div class="skills-box">
       <div class="skills-title">
       <div class="skills-img">
        <img src="https://i.postimg.cc/ZRT9Z4Y1/icons8-vue-js-480.png" alt="" class="skills-icons">
        </div>
        <h3>VUE.JS</h3>
        </div>
        
       </div>

       <div class="skills-box">
       <div class="skills-title">
       <div class="skills-img">
        <img src=" https://i.postimg.cc/vB1MFKFW/fl-studio-icon.png" alt="" class="skills-icons">
        </div>
        <h3>FL STUDIO</h3>
        </div>
    
       </div>

       
       
       </div>
    
       
     </div>


    </div>
  
  
  </template>
  
  <script>

  import NavbarC from '@/components/NavbarC.vue'
  
  export default {
    name: "HomeView",
    components: {

      NavbarC
    }
};
  
  </script>
  
  <style scoped>
main {
  min-height: 100vh;
  background: linear-gradient(rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 1)),
  url(https://i.postimg.cc/Tw99zpwZ/indivar-kaushik-gc-A0-W3-OOOts-unsplash.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
}

p,h2,h3,h3,h4,h5{
  font-family: 'Fjalla One', sans-serif;
}
  #heading-skillspage {
  font-family: 'Fjalla One', sans-serif;
}


.skills-section{
padding-top: 20px;
}

.skills-header{
text-align: center;
color: #fff;
padding: 1rem;
position: relative;
}

.skills-header:after{
content: '';
position: absolute;
bottom: 0;
left: 50%;
transform: translateX(-50%);
width: 100px;
height: 4px;
background-color: #222021;
border-radius: 2px;
}

.skills-container{
display: grid;
grid-tempLate-columns: repeat(5, 1fr);
justify-content:center;
align-items:center;
text-align: center;
grid-gap:1rem;
padding: 1rem 80px;
font-size: 1.2rem;
}

.skills-box{
padding: 1rem;
color: #000;
cursor:pointer;
}

.skills-box:hover > .skills-title:after, 
.skills-box:hover > .skills-title:before{
width: 30px;
}

.skills-box:hover .skills-img{
transform: translateX(-20px);
}

.skills-title{
display:flex;
flex-direction: column;
align-items:center;
padding: 0.5rem;
margin-bottom: 0.5rem;
position: relative;
}

.skills-title:after{
content: '';
position:absolute;
bottom: 0;
rigth: 50%;
width:20px;
height:4px;
border-radius: 2px 0 0 2px;
background-color: #222021;
transition: .5s;
}

.skills-title:before{
content: '';
position:absolute;
bottom: 0;
left: 50%;
width:100px;
height:4px;
border-radius: 0 2px 2px 0;
background-color: #222021;
}

.skills-icons{
width:50px;
z-index:2;
}

.skills-img{
width:100px;
height:100px;
position: relative;
border-radius: 45px;
background-color: #fff;
display:flex;
justify-content:center;
align-items:center;
transition: .5s;
}

.skills-img:after{
content: '';
position:absolute;
top:0;
left: 0;
width:50%;
height:90px;
/* background: rgba(100, 100, 100, 0.5); */
border-radius: 45px 0 0 45px;
}
.skills-title h3{
color: #333;
margin-top: 0.5rem;
}
@media screen and (max-width:990px){
 .skills-container{
 grid-tempLate-columns: repeat(2, 1fr);
 padding: 2rem 50px;
 }
}

@media screen and (max-width:650px){
 .skills-container{
 grid-tempLate-columns:2fr;
 padding: 2rem 50px;
 }
}


  </style>
  