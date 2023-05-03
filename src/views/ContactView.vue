<template>
  <main>
    <NavbarC />
    <section class="contact-main">
      <section id="contact">
        <div class="container-fluid img-fluid">
          <div class="row d-flex flex-column flex-md-row">
            <div loading="lazy" class="img1">
              <div class="contact-text col">
                <h1
                  id="heading-contact"
                  style="padding-top: 15rem; font-size: 50px"
                  class="lead display-6">
                  CONTACT
                </h1>
              </div>
            </div>
          </div>
        </div>
      </section>
    </section>
  </main>

  <div>
    <section class="container">
      <div class="contact">
        <h2 class="text-dark pt-4 pb-3">Contact me</h2>
        <!-- <form @submit.prevent="userRegister">
          <br />

          <div class="form-outline">
            <label class="text-dark" for="#firstname" style="font-size: 20px"
              >Name</label
            >
            <input
              id="firstname"
              class="form-control"
              name="firstName"
              type="text"
              placeholder="Enter your name"
              required
            />
          </div>
          <div>
            <label class="text-dark" for="#number" style="font-size: 20px"
              >Number</label
            >
            <input
              id="surname"
              class="form-control"
              name="surname"
              type="number"
              placeholder="Enter your Number"
              required
            />
          </div>

          <div>
            <label class="text-dark" for="#Email" style="font-size: 20px"
              >Email</label
            >
            <input
              id="surname"
              class="form-control"
              name="surname"
              type="text"
              placeholder="Enter your Email"
              required
            />
          </div>

          <div>
            <label class="text-dark" for="#surname" style="font-size: 20px"
              >Surname</label
            >
            <input
              id="surname"
              class="form-control"
              name="surname"
              type="text"
              placeholder="Enter your surname"
              required
            />
          </div>

          <div>
            <label class="text-dark" for="#message" style="font-size: 20px"
              >Message</label
            >
            <textarea
              name="message"
              class="form-control"
              cols="45"
              rows="5"
              placeholder="Enter your message"
              required
            ></textarea>
          </div>
          <div class="button">
            <input type="submit" value="submit" />
          </div>
          <br />
        </form> -->
      </div>

      <div class="row g-3">
     
        <form action="">
            
        </form>
            <div class="col">
              <div class="form-outline">
                <label class="text-dark" for="#firstname" style="font-size: 20px"
                  >Name</label
                >
                <input
                  id="firstname"
                  class="form-control"
                  name="firstName"
                  type="text"
                  placeholder="Enter your name"
                  required
                />
              </div>
    
              <div>
                <label class="text-dark" for="#Email" style="font-size: 20px">Email</label>
                <input id="surname" class="form-control" name="surname" type="text" placeholder="Enter your Email" required/>
              </div>
            </div>
            <div class="col">
              <div>
                <label class="text-dark" for="#surname" style="font-size: 20px"
                  >Surname</label
                >
                <input  id="surname" class="form-control" name="surname" type="text" placeholder="Enter your surname" required
                />
              </div>
    
              <div>
                <label class="text-dark" for="#number" style="font-size: 20px">Number</label>
                <input id="surname" class="form-control" name="surname" type="number" placeholder="Enter your Number" required/>
              </div>
            </div>
            <div>
              <label class="text-dark" for="#message" style="font-size: 20px"
                >Message</label
              >
              <textarea
                name="message"
                class="form-control"
                cols="45"
                rows="5"
                placeholder="Enter your message"
                required
              ></textarea>
            </div>
       
        <div class="button">
          <input type="submit" value="submit" />
        </div>
      </div>
    </section>
  </div>
</template>
<script>
import NavbarC from "@/components/NavbarC.vue";
export default {
  components: { NavbarC },
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
}

#heading-contact {
  font-family: "Fjalla One", sans-serif;
}

p {
  font-size: 19px;
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
  border-radius: 4px;
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
</style>
