<template>
  <div>

    <section class="container">
      <div class="contact">
        <div class="skills-section">
          <div class="skills-header">
            <h2 class="skills-heading text-dark">CONTACT ME</h2>
          </div>
        </div>
        <h2 class="text-dark pt-4 pb-3"></h2>
        <form action="https://formspree.io/f/xayzrrjb" method="POST" target="_blank">
          <br />

          <div class="form-outline">
            <label class="text-dark" for="firstname" style="font-size: 20px; padding-top: 1rem; display: flex;">Name</label>
            <input
              id="firstname"
              class="form-control"
              v-model="formData.firstName"
              type="text"
              name="firstName"
              placeholder="Enter your name"
              required
            />
          </div>

          <div>
            <label class="text-dark" for="surname" style="font-size: 20px; padding-top: 1rem; display: flex;">Surname</label>
            <input
              id="surname"
              class="form-control"
              v-model="formData.surname"
              type="text"
              name="surname"
              placeholder="Enter your surname"
              required
            />
          </div>

          <div>
            <label class="text-dark" for="email" style="font-size: 20px; padding-top: 1rem; display: flex;">Email</label>
            <input
              id="email"
              class="form-control"
              v-model="formData.email"
              type="email"
              name="email"
              placeholder="Enter your email"
              required
            />
          </div>


          <div>
            <label class="text-dark" for="number" style="font-size: 20px; padding-top: 1rem; display: flex;">Number</label>
            <input
              id="number"
              class="form-control"
              v-model="formData.number"
              type="number"
              name="phoneNumber"
              placeholder="Enter your number"
              required
            />
          </div>
      

          <div>
            <label class="text-dark" for="message" style="font-size: 20px; padding-top: 1rem; display: flex;">Message</label>
            <textarea
              name="message"
              v-model="formData.message"
              class="form-control"
              cols="45"
              rows="5"
              placeholder="Enter your message"
              required
            ></textarea>
          </div>

          <div class="button" style="padding-top: 1rem;">

            <input  class="linktr__goal r-link" target="_blank" type="submit" style="  background-color: #1D1D1D;
    border-radius: 20px;" value="Submit" />
          </div>

          <br />
        </form>
      </div>
    </section>

  


  </div>
</template>

<script>
export default {
  data() {
    return {
      formData: {
        firstName: '',
        phoneNumber: '',
        email: '',
        surname: '',
        message: ''
      }
    };
  },
  methods: {
    userRegister() {
      fetch('https://formspree.io/your-email@example.com', {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json'
        },
        body: JSON.stringify(this.formData)
      })
        .then(response => {
          if (response.ok) {
            // Form submission successful
            console.log('Form submitted successfully!');
            // You can reset the form or show a success message here
          } else {
            // Form submission failed
            console.error('Form submission failed.');
          }
        })
        .catch(error => {
          console.error('Error:', error);
        });
    }
  }
};
</script>


  <style scoped>
  @import url("https://fonts.googleapis.com/css2?family=Fjalla+One&display=swap");
  
  /* p */
  @import url("https://fonts.googleapis.com/css2?family=Rubik&display=swap");
  
  main {
    min-height: 100vh;
    background: linear-gradient(rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 1)),
    url(https://i.postimg.cc/Wp80HxDG/rupixen-com-yd-Teom-wtoc-unsplash.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position: center;
    background-attachment: fixed;
  }
  
  #heading-contact {
    font-family: "Fjalla One", sans-serif;
  }
  
  p {
    font-size: 19px;
    font-family: "Rubik", sans-serif;
  }

  ::placeholder label{
    font-family: "Rubik", sans-serif;
  }

  input {
    font-family: "Rubik", sans-serif;
  }

  label {
    font-family: "Rubik", sans-serif;
  }
  
  .text-dark {
    font-family: "Fjalla One", sans-serif;
    font-style: normal;
    font-weight: 500;
  }
  
  .contact {
    padding: 1rem;
  }
  input[type="submit"] {
    color: rgb(255, 255, 255);
    background-color: #808080;
    padding: 12px 20px;
    border: none;
    border-radius: 10px;
  }
  input[type="text"] {
    width: 100%;
    padding: 10px 20px;
    margin: 8px 0px;
    box-sizing: border-box;
  }
  input[type="number"] {
    width: 100%;
    padding: 10px 20px;
    margin: 8px 0px;
    box-sizing: border-box;
  }
  /* input:hover[type=text] {
      border: none;
      border: 4px;
  } */
  textarea {
    width: 100%;
    height: 150px;
    padding: 12px 20px;
    box-sizing: border-box;
    border-radius: 4px;
    resize: none;
  }
  /* textarea:hover {
      border: none;
      box-sizing: border-box;
      border-radius: 4px;
      
  } */
  .button {
    padding-bottom: 2rem;

  }

  .skills-section{
padding-top: 20px;
width: 100%;
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

.bg-dark{
  border-radius: 50%;
  
}
.linktr__goal{
  background-color: rgb(0, 0, 0);
  color: rgb(8, 49, 112);
  box-shadow: rgb(8 49 112 / 24%) 0px 2px 8px 0px;
  border-radius: 2rem;
  padding: .75rem 1.5rem;
  margin: auto;
}

.r-link{
    --uirLinkDisplay: var(--rLinkDisplay, inline-flex);
    --uirLinkTextColor: var(--rLinkTextColor);
    --uirLinkTextDecoration: var(--rLinkTextDecoration, none);

    display: var(--uirLinkDisplay) !important;
    color: var(--uirLinkTextColor) !important;
    text-decoration: var(--uirLinkTextDecoration) !important;
}

.button {
    padding-top: 1rem;
  }

  form input:focus {
    outline-color: red;
  }

  </style>
  