<template>

  <section id="about" >
    <div class="skills-section">
      <div class="skills-header">
        <h2 class="skills-heading text-dark">ABOUT</h2>
      </div>
    </div>

   

<div class="container" style="min-height: 80vh; max-width: 100%">
  <div class="row">
    <div class="col-md-6 text-dark pt-2 my-img">
      <img
        src="https://i.postimg.cc/d09dynK8/My-project.png"
        alt=""
        style="
          border-radius: 50%;
          padding-left: 2rem;
          width: 100%;
          max-width: 30rem;
          border: 1px solid;
          padding: 10px;
          margin-top: 12px;
          box-shadow: 0 5px 10px rgb(0, 0, 0);
        "
      />
    </div>
    <div class="col-md-5 text-dark" style="margin: auto; padding-top: 3rem">
      <p>
        Hello, I'm Brogan Gys, a <b>passionate</b> 21-year-old front-end web
        developer with a <b>love for coding</b>, particularly in the front-end
        field. I take great pleasure in styling, designing, and enhancing
        web projects to create captivating user experiences. <b>Building</b>
        strong, enduring relationships with both team members and clients is
        of utmost importance to me. I am known for my approachable nature,
        <b>adaptability</b>, and willingness to support project goals
        wholeheartedly. My positive attitude and sense of humor foster a
        friendly and <b>productive</b> working environment. In my spare time, you
        can find me indulging in my other passions: music production and
        playing soccer. I believe in maintaining a healthy, balanced life to
        fuel creativity and success.
      </p>

      <!-- <div
        class="container w-100 text-center"
        style="box-shadow: 0 5px 10px rgb(0, 0, 0); border-radius: 20px 20px 20px 20px;"
      >
        <div class="row">
          <div class="w-100"></div>

          <div class="col-6 col-sm-6 test">
            <i class="fa fa-phone" style="font-size: 15px"></i>
            <span class="number" style="font-size: 16px"><span  style="padding-right: 7px;"></span>069 516 6923</span>
          </div>
          <div class="col-6 col-sm-6 test">
            <i class="fa fa-envelope" style="color: #222021; font-size: 17px"></i>
            <span style="font-size: 16px"> <span style="padding-right: 7px;"></span>prodbrogy@gmail.com</span>
          </div>
        </div>
      </div> -->

      <button @click="toggleCollapsible" class="collapsible">Click On Me</button>
  <div class="content"  v-if="collapsibleOpen">
    <p style="font-size: 17px !important;">Email: brogangys2@gmail.com</p><br>
    <p style="font-size: 17px !important;">Phone Number: 069 516 6923 </p><br>
    <p style="font-size: 17px !important;">Located In: Belhar </p><br>

  </div>
      


    <!-- Optional: Add an empty column for spacing -->
    <div class="col-md-1"></div>
  </div>
</div>
</div>
  


  </section>
<!-- 
  <section class="testimonial-main">
    <section id="testimonial">
      <div class="container-fluid img-fluid">
        <div class="row d-flex flex-column flex-md-row">
          <div loading="lazy" class="img1">
            <div class="testimonial-text col">
              <h1
                id="heading-testimonial"
                style="padding-top: 20rem; font-size: 50px"
                class="lead display-6"
              >
                TESTIMONIALS
              </h1>
            </div>
          </div>
        </div>
      </div>
    </section>
  </section> -->

  <section id="testimonials">
    <div class="skills-section">
      <div class="skills-header">
        <h2 class="skills-heading text-dark">TESTIMONIALS</h2>
      </div>
    </div>

    <div class="testimonials text-center">
  <div class="row" style="gap: 2rem">
    <div v-for="item in info" :key="item" class="card text-center">
      <i class="fa fa-quote-left fa-3x card-img-top rounded-circle" aria-hidden="true"></i>
      <img :src="item.image" style="height: 100%; width: 100%; border-radius: 50%; padding: 5px" class="image-fluid" />
      <div class="overlay">
        <div class="text">
          <cite title="Source Title">
            <h5>
              <div style="padding-top: 30px;">{{ item.name }}</div>
            </h5>
          </cite>

          

          <br />
          <h4 style="">{{ item.reference }}</h4>
          <div class="card-body blockquote">
            <p class="card-text" style=" padding: 10px">
              {{ item.message }}
            </p>
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
export default {
  name: "HomeView",
  components: {
    // MenuC
  },

  data() {
    return {
      info: [
        {
          name: "Joel Mukanya",
          reference: "Lecturer",
          image: "https://i.postimg.cc/hG0D4dbZ/Joel-Profile.jpg",
          message:
            "Brogan is a very creative, go-getter, and well-behaved student who is committed at the task at hand and always works well with groups / teams.",
        },
        {
          name: "Meezaan Davids",
          reference: "Colleague",
          image:
            "https://i.postimg.cc/BbGgfnF1/Meezaan-Profile-black-and-white.jpg",
          message:
            "Brogan has a really bright and innovative mind when it comes to the design of his projects. Brogan to the eye is very introverted but once he opens up he is totally the opposite.",
        },
        {
          name: "Imraan Bernksen",
          reference: "Colleague",
          image: "https://i.postimg.cc/4yrkQ6T5/imraan-black-and-white.jpg",
          message:
            "Brogan has a good judge of character, he is a very friendly person to be around. He is also very passionate about his music producing, I view him as a smart and knowledgeable guy.",
        },
        {
          name: "Cassidy Lawrence",
          reference: "Colleague",
          image:
            "https://i.postimg.cc/8CQsHfgW/Picsart-23-05-04-09-12-42-406.jpg",
          message:
            "Brogan is an extremely committed worker. He does not let go of his attention till the job is done. He works well with others as a team and is always eager to lend a hand when needed. He fosters a great working environment by being extremely respectful and understanding of everyone around him.",
        },
        {
          name: "Mueen Slamat",
          reference: "Colleague",
          image: "https://i.postimg.cc/YSWY2wMN/mueen-black-and-white.jpg",
          message:
            "Brogan is a kind-hearted, hard-working, humorous team player. He's a passive guy. His design thinking is top-notch. His coding abilities only get better. He supports his peers and motivates others as well as himself.",
        },
        {
          name: "Lazola Makubalo",
          reference: "Colleague",
          image: "https://i.postimg.cc/qMRx8Pmj/Lazola-black-and-white.jpg",
          message:
            "Brogan likes learning new stuff, he is a team player and he is someone who is always on time. I can assure you that he can be a great asset to your company.",
        },
      ],
      collapsibleOpen: false, // Add this variable to control the collapsible content
    };
  },

  methods: {
    toggleCollapsible() {
      // Toggle the value of collapsibleOpen to show/hide the content
      this.collapsibleOpen = !this.collapsibleOpen;
    },
  },

  mounted() {
    // This code will run after the component is mounted
    var coll = document.getElementsByClassName("collapsible");
    var i;

    for (i = 0; i < coll.length; i++) {
      coll[i].addEventListener("click", function () {
        this.classList.toggle("active");
        var content = this.nextElementSibling;
        if (content.style.display === "block") {
          content.style.display = "none";
        } else {
          content.style.display = "block";
        }
      });
    }
  },
};

</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Fjalla+One&display=swap");

/* p */
@import url("https://fonts.googleapis.com/css2?family=Rubik&display=swap");

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
  font-family: "Fjalla One", sans-serif;
}

.skills-section {
  padding-top: 20px;
}

.skills-header {
  text-align: center;
  color: #fff;
  padding: 1rem;
  position: relative;
  font-family: "Fjalla One", sans-serif;
}


.skills-header:after {
  content: "";
  position: absolute;
  bottom: 0;
  left: 50%;
  transform: translateX(-50%);
  width: 100px;
  height: 4px;
  background-color: #222021;
  border-radius: 2px;
}

p {
  font-size: 19px;
  font-family: "Rubik", sans-serif;
  text-align: start;
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
  font-family: "Fjalla One", sans-serif;
}

.test{
  border-radius: 20%;
}

.about-heading {
  margin: auto;
  font-family: "Fjalla One", sans-serif;
  font-style: normal;
  font-weight: 500;
  font-size: 40px;
  padding-top: 2rem;
  padding-bottom: 2rem;
}

/* Style the button that is used to open and close the collapsible content */
.collapsible {
  background-color: #eee;
  color: #000000;
  cursor: pointer;
  padding: 18px;
  width: 100%;
  border: none;
  text-align: left;
  outline: none;
  font-size: 15px;
  font-family: "Fjalla One", sans-serif;
}

/* Add a background color to the button if it is clicked on (add the .active class with JS), and when you move the mouse over it (hover) */
.active, .collapsible:hover {
  background-color: #ccc;
}

/* Style the collapsible content. Note: hidden by default */
.content {
  padding: 0 18px;
  display: none;
  overflow: hidden;
  background-color: #f1f1f1;
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
  .icons-about {
    display: flex !important ;
    gap: 50px;
    padding-left: 19px;
    padding-top: 1rem !important;
    font-size: 35px !important;
    margin-left: 2rem;
  }

  .fa-at .fa-phone {
    font-size: 15px !important;
  }

  .about-heading {
    padding-bottom: 0 !important;
  }

  .container .my-img {
    padding-bottom: 2rem;
  }
}

@media (max-width: 450px) {
  .number {
    display: block !important;
  }
}

@media (max-width: 300px) {
  .icons-about {
    display: flex !important ;
    margin-left: 2rem;
  }
}

/* CSS for large screens */
@media (min-width: 700px) {
    /* Adjust the image size */
    .my-img img {
      max-width: 30rem;
    }

    /* Center the contact details */
    .contact-details {
      text-align: center;
    }

    /* Remove padding-top on contact details */
    .contact-details p {
      padding-top: 0;
    }

    /* Adjust padding for social icons */
    .icons-about {
      padding-top: 1rem;
      gap: 4rem;
    }
  }

  /* CSS for medium screens */
  @media (max-width: 699px) {
    /* Reduce the image size */
    .my-img img {
      max-width: 100%;
    }

    /* Center the contact details */
    .contact-details {
      text-align: center;
    }

    /* Reduce padding for social icons */
    .icons-about {
      padding-top: 0.5rem;
      gap: 2rem;
    }
  }

  /* CSS for small screens */
  @media (max-width: 380px) {
    /* Reduce the size of social icons */
    .icons-about {
      font-size: 18px;
    }

    /* Center the social icons */
    .icons-about {
      justify-content: center;
    }
  }

/* ############################################################################################################################################
  -------------------------------Testimonials------------------------------------------------
  ############################################################################################################################################ */

.testimonial-main {
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

.background-fade {
  background: linear-gradient(rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 1));
}

#heading-testimonial {
  font-family: "Fjalla One", sans-serif;
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
  transition: 0.5s ease;
}
.card:hover .overlay {
  height: 100%;
  border-radius: 50%;
}
.text {
  padding: 0;
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

@media (max-width: 400px) {
  .icons {
    display: flex !important ;
    gap: 50px;
    padding-top: 1rem !important;
    font-size: 35px !important;
  }
}

@media (max-width: 490px) {
  .card {
    width: 15rem;
    height: 15rem;
  }

  .card img {
    padding: 5px;
  }

  .testimonials {
    padding: 50px;
  }

  .testimonials .card {
    margin-top: 30px;
  }
  .blockquote p {
    font-size: 10px;
    /* padding: 1rem; */
  }

  .text h4 {
    font-size: 16px;
    /* padding: 0.5rem; */
  }

  .text cite {
    font-size: 12px;
    margin-bottom: 2rem;
  }

  .card-text {
    padding: 0 !important;
  }
}


</style>
