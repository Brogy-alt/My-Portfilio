<template>
  <main>
    <NavbarC />
    <section id="about">
      <div class="container-fluid img-fluid">
        <div class="row d-flex flex-column flex-md-row">
          <div loading="lazy" class="img1">
            <div class="about-text col">
              <h1 id="heading-aboutpage" style="padding-top: 15rem; font-size: 50px" class="lead display-6">
                ABOUT & TESTIMONIALS
              </h1>
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>


  <section id="about">

    <div class="about-text-section">
      <h2 class="about-heading" >About me</h2>

    </div>

    



    <div class="container" style="min-height: 80vh; max-width: 100%;" >
      <div class="row">
        <div class="col-md text-dark pt-2 my-img">
         <img src="https://i.postimg.cc/d09dynK8/My-project.png" alt="" style="border-radius: 50%; padding-left: 2rem;
          width: 27rem; border: 1px solid; padding: 10px;  box-shadow: 0 5px 10px rgb(0, 0, 0);; ">
        </div>
        <div class="col-md text-dark" style="margin: auto ; padding-top: 3rem; ">
          <p>I am a 21 year old web developer who has recently <b>completed</b> my learning phase at
            Life Choices Academy and <b>successfully</b>
            completed the course and is now a <b>full stack developer</b>. I am someone who prefers creating long lasting relationships with people 
            I meet , I'm someone who has a good sense of humour and Im someone who also tries to make everyone feel comfortable with me and their surroundings ,   
            I see my self as a <b>team player</b> who is willing to help and adjust to meet the required needs also lastly , 
            I have a passion for music and I have been producing music since 2018 and In my spare time I create music and youtube content thats related to my music.</p>

            <div class="container w-100 text-center" style="  box-shadow: 0 5px 10px rgb(0, 0, 0);" >
          <div class="row">
            

            <!-- Force next columns to break to new line -->
            <div class="w-100" ></div>

            <div class="col-6 col-sm-6 "><i class="fa-solid fa-phone" style="font-size: 15px;"></i> <span style="font-size: 16px;">No.069 516 6923</span> </div>
            <div class="col-6 col-sm-6 "><i class="fa-solid fa-at" style="font-size: 15px;"></i> <span style="font-size: 16px;">brogangys2@gmail.com</span>  </div>
          </div>
        </div>
        </div>

        <div class="col-md text-dark pt-2">
          <div class="row">
                    <ul class="icons" style="font-size: 50px; list-style-type:none; padding-top:5rem">
                        <li><a href=""><i id="linkedin" class="fa fa-linkedin text-dark" style="padding-bottom: 2rem;"></i></a></li>
                        <li><a href="https://www.instagram.com/?__coig_restricted=1"><i id="ig" class="fa fa-instagram text-dark" style="padding-bottom: 2rem;"></i></a></li>
                        <li><a href="https://www.youtube.com/"><i id="yt" class="fa fa-youtube text-dark" style="padding-bottom: 2rem;"></i></a></li>
                        <li><a href="..."><i id="github" class="fa-brands fa-github text-dark" style="padding-bottom: 2rem;"></i></a></li>
                    </ul>
            </div>
        </div>
      </div>
    </div>


  </section>

  <section class="testimonial-main">
    <section id="testimonial">
      <div class="container-fluid img-fluid">
        <div class="row d-flex flex-column flex-md-row">
          <div loading="lazy" class="img1">
            <div class="testimonial-text col">
              <h1 id="heading-testimonial" style="padding-top: 19rem; font-size: 50px" class="lead display-6">
                TESTIMONIALS
              </h1>
            </div>
          </div>
        </div>
      </div>
    </section>
  </section>

  
  <section id="testimonials">
        <h6 class="heading">Testimonials</h6>
        <div class="testimonials text-center">
              <div class="row" style="gap: 2rem">
                    <div v-for="item in info" :key="item" class="card text-center">
                        <i class="fa fa-quote-left fa-3x card-img-top rounded-circle" aria-hidden="true"></i>
                      <img :src="item.image" style="height: 100%;width: 100%;border-radius: 50%;padding: 20px;" class="image-fluid">
                    <div class="overlay">
                      <div class="text">
                          <cite title="Source Title"><b>{{ item.name }}</b></cite>
                          <br>
                          <h4>{{ item.reference }}</h4>
                          <div class="card-body blockquote">
                            <p class="card-text" style="font-family: 'Fjalla One', sans-serif; padding: 2rem;">{{ item.message }}</p>
                          </div>
                      </div>
                    </div>
                </div>
                  </div>
             </div>
      <div class="background-fade"></div>
  </section>

</template>

<script>



import NavbarC from '@/components/NavbarC.vue'

export default {
  name: "HomeView",
  components: {
 
    NavbarC
  },
  data() {
        return {
            info : [
                {
                    name: 'Joel Mukanya',
                    reference: 'Lecturer',
                    image: "https://i.postimg.cc/hG0D4dbZ/Joel-Profile.jpg",
                    message: 'Brogan is a very creative, go-getter, and well-behaved student who is committed at the task at hand and always works well with groups / teams.'
                }, 
                {
                    name: 'Meezaan Davids',
                    reference: 'Peer',
                    image: "https://i.postimg.cc/QdNGkx2v/Meezaan-Profile-black-and-white.jpg",
                    message: 'Brogan has a really bright and innovative mind when it comes to the design of his projects. Brogan to the eye is very introverted but once he opens up he is totally the opposite.'
                },
                {
                    name: 'Imraan Bernksen',
                    reference: 'Peer',
                    image: "https://i.postimg.cc/4yrkQ6T5/imraan-black-and-white.jpg",
                    message: 'Brogan has a good judge of character, he is a very friendly person to be around.He is also very passionate about his music producing, I view him as a smart and knowledgeable guy.'
                },
                {
                    name: 'Cassidy Lawrence',
                    reference: 'Peer',
                    image: "https://i.postimg.cc/3Np4BZvr/cassidy-black-and-white.jpg",
                    message: 'Brogan is an extremely committed worker. He doesnt let go of his attention till the job is done. He works well with others as a team and is always eager to lend a hand when needed. He fosters a great working environment by being extremely respectful and understanding of everyone around him. Hes willing to take on challenges and would be a great asset to any team.'
                },
                {
                    name: 'Mueen Slamat',
                    reference: 'Peer',
                    image: "https://i.postimg.cc/P573pXTW/mueen-black-and-white.jpg",
                    message: 'Meezaan is a chilled and honest guy.He always gives 100% to anything he faces. He will always be willing to help the next person. He is a goal driven individual. A real "COOL" guy.'
                },
                {
                    name: 'Lazola Makubalo',
                    reference: 'Peer',
                    image: "https://i.postimg.cc/qMRx8Pmj/Lazola-black-and-white.jpg",
                    message: 'Brogan likes learning new stuff, he is a team player and he is someone who is always on time. I can assure you that he can be a great asset to your company.'
                }
            ]
        }
}

};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Fjalla+One&display=swap');

/* p */
@import url('https://fonts.googleapis.com/css2?family=Rubik&display=swap');

main {
  background: linear-gradient(rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 1)),
  url(https://i.postimg.cc/qM0WdYMm/miguel-alcantara-lt-Be-ID9-Bw-I-unsplash.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  height: auto;

}

h2,
h3,
h4,
h5 {
  color: black;
}

p{
   font-size: 19px;
   font-family: 'Rubik', sans-serif;
}

#about {
  min-height: 100vh;
  width: 100vw;

}

.container {
  
  padding: 10px;
  overflow: hidden;
  box-sizing: border-box;

}

.container img {
  max-width: 100%; 
}

.container p {
  word-wrap: break-word; 
}




#heading-aboutpage {
  font-family: 'Fjalla One', sans-serif;


}

.about-heading {
  margin: auto;
  font-family: 'Fjalla One', sans-serif;
  font-style: normal;
  font-weight: 500;
  font-size: 40px;
  padding-top: 2rem;
  padding-bottom: 2rem;

}



#linkedin:hover {
  transform: scale(1.1);
  transition: all ease 500ms;
}

#ig:hover {
  transform: scale(1.1);
  transition: all ease 500ms;
}

#yt:hover {
  transform: scale(1.1);
  transition: all ease 500ms;
}

#github:hover {
  transform: scale(1.1);
  transition: all ease 500ms;
}

@media (max-width: 400px) {
  .icons {
    display: flex !important ;
    gap: 50px;
    padding-left: 19px;
    padding-top: 1rem !important;
    font-size: 35px !important;;
   
  }

.fa-at .fa-phone{
font-size: 15px !important;
} 

  .about-heading{
    padding-bottom: 0 !important; 
  }

  .container .my-img{
    padding-bottom: 2rem;
    
  }
}

/* ############################################################################################################################################
-------------------------------Testimonials------------------------------------------------
############################################################################################################################################ */


.testimonial-main{

  height: 100vh;
  width: 100%;
  background: linear-gradient(rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 1)),
  url(https://i.postimg.cc/dVvMXds3/sam-balye-w1-Fw-Dv-Ire-ZU-unsplash.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  background-attachment: fixed;

}

#testimonials {
  height: auto;
  width: 100%;
 

}

.background-fade{
  background: linear-gradient(rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 1));
  
}

#heading-testimonial{
  font-family: 'Fjalla One', sans-serif;

}

.card {
    margin: auto;
    justify-content: center;
    padding: 20px;
    width: 30rem;
    height: 30rem;
    background-color: transparent;
    border-radius: 50%;
    box-shadow: 0 5px 10px rgb(0, 0, 0);
    
}
/* .card-text, b, h4 {
    font-family: 'Merienda', cursive;
    font-size: 14px;
} */
.overlay {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    color: black;
    background: rgba(255, 255, 255, 0.5);
    backdrop-filter: blur(50px);
    overflow: hidden;
    width: 100%;
    height: 0;
    transition: .5s ease;
  }
  .card:hover .overlay {
    height: 100%;
    border-radius: 50%;
  }
  .text {
     padding: 20px;
  }
.testimonials {
    padding: 100px;
  }
  .testimonials h3 {
    margin-bottom: 20px;
  }
  .testimonials .card {
    border: 3px rgb(0, 0, 0) solid !important;
    transition: 0.5s;
    margin-top: 60px;
  }
  .testimonials .card i {
    background-color: rgb(0, 0, 0);
    color: #ffffff;
    width: 75px;
    height: 75px;
    line-height: 75px;
    margin: -60px auto 0 auto;
  }


</style>

