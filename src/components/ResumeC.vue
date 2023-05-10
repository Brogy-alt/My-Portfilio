<template>
    <div class="skills-page">
      <main>
        <section id="skills-page">
          <div class="container-fluid ">
            <!-- <MenuC/> -->
            <div class="row d-flex flex-column flex-md-row">
              <div loading="lazy" class="img1 img-fluid">
                <div class="home-text col">
                  <h1 
                    id="heading-skillspage"
                    style="padding-top: 15rem; font-size: 50px"
                    class="lead display-6">
                    RESUME
                  </h1>
                </div>
              </div>
            </div>
          </div>
        </section>
      </main>
      

      <div class="skills-section">
    <div class="skills-header">
     <h2 class="skills-heading text-dark">TIMELINE</h2>   
     </div> 
     </div>

      <div class="page">
  <div class="timeline">
    <div class="timeline__group">
      <span class="timeline__year time" aria-hidden="true">2023</span>
      <div class="timeline__cards">
        <div class="timeline__card card">
          <header class="card__header">
            <time class="time" datetime="2008-02-02">
 
              <span class="time__month">Currently</span>
            </time>
          </header>
          <div class="card__content">
            <p>I am an intern learning in the Life Choices Studio about UI/UX, SEO and wordpress</p>
          </div>
        </div>
     
      </div>
    </div>
    <div class="timeline__group">
      <span class="timeline__year time" aria-hidden="true">2022</span>
      <div class="timeline__cards">
        <div class="timeline__card card">
          <header class="card__header">
            <time class="time" datetime="2008-07-14">
              <span class="time__month">October</span>
            </time>
          </header>
          <div class="card__content">
            <p>I started my journey at Life Choices Academy and completed the academy phase in January 2023</p>
          </div>
        </div>
      </div>
    </div>
    <div class="timeline__group">
      <span class="timeline__year time" aria-hidden="true">2016</span>
      <div class="timeline__cards">
        <div class="timeline__card card">
          <header class="card__header">
            <time class="time" datetime="2008-08-18">
              <span class="time__month">High school</span>
            </time>          
          </header>
          <div class="card__content">
            <p>Attended Symphony High School from 2016 and graduated and passed with a bachelors in 2021, highlights from my time there was winning awards
               or certificates for CAT and I was nominated to be a prefect and I was one during my matric year.</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
<div class="CV">
  <!-- <a href="https://cssisntmagic.substack.com" target="_blank" >Download My CV</a> -->

  <button id="download-btn" class="linktr__goal r-link" @click="downloadCV">Download My CV</button>

</div>


      
    </div>
  
  
  </template>
  
  <script>

//   import MenuC from '@/components/MenuC.vue'
  
  export default {
    name: "HomeView",
    components: {

    //   MenuC
    },
    methods: {
    downloadCV() {
      const link = document.createElement('a');
      link.href = 'https://drive.google.com/file/d/1ZSx5pq4RdCV0U6Y_g6PTe57TmXQjEE7i/view?usp=sharing'; // Replace 'path_to_your_cv_file.pdf' with the actual path to your CV file
      link.download = 'BroganGys-CV.pdf'; // Replace 'your_cv_file_name.pdf' with the desired name for the downloaded file
      link.click();
    }
  }
};
  
  </script>
  
  <style scoped>
main {
  min-height: 100vh;
  background: linear-gradient(rgba(255, 255, 255, 0.1), rgba(0, 0, 0, 1)),
  url(https://i.postimg.cc/HjGV3tmH/mario-gogh-v-Hk-GKvk-S6-No-unsplash.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
}
  

 

  #heading-skillspage {
  font-family: 'Fjalla One', sans-serif;
}

p,h2,h3,h3,h4,h5{
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
font-family: 'Fjalla One', sans-serif;
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

/*
!!!!
This pen is being refactored
!!!!
*/

/*
=====
DEPENDENCES
=====
*/

.r-title{
  margin-top: var(--rTitleMarginTop, 0) !important;
  margin-bottom: var(--rTitleMarginBottom, 0) !important;
}


p:not([class]){
  line-height: var(--cssTypographyLineHeight, 1.78);
  margin-top: var(--cssTypographyBasicMargin, 1em);
  margin-bottom: 0;
}

p:not([class]):first-child{
  margin-top: 0;
}

/*
text component
*/

.text{
  display: var(--textDisplay, inline-flex);
  font-size: var(--textFontSize, 1rem);  
}

/*
time component
*/

/*
core styles
*/

.time{
  display: var(--timeDisplay, inline-flex);
}

/*
extensions
*/

.time__month{
  margin-left: var(--timelineMounthMarginLeft, .25em);
}

/*
skin
*/

.time{
  padding: var(--timePadding, .25rem 1.25rem .25rem);
  background-color: var(--timeBackgroundColor, #f0f0f0);

  font-size: var(--timeFontSize, .75rem);
  font-weight: var(--timeFontWeight, 700);
  text-transform: var(--timeTextTransform, uppercase);
  color: var(--timeColor, currentColor);
}

/*
card component
*/

/*
core styles
*/

.card{
  padding: var(--timelineCardPadding, 1.5rem 1.5rem 1.25rem);
}

.card__content{
  margin-top: var(--cardContentMarginTop, .5rem);
}

/*
skin
*/

.card{
  border-radius: var(--timelineCardBorderRadius, 2px);
  border-left: var(--timelineCardBorderLeftWidth, 3px) solid var(--timelineCardBorderLeftColor, var(--uiTimelineMainColor));
  box-shadow: var(--timelineCardBoxShadow, 0 1px 3px 0 rgba(0, 0, 0, .12), 0 1px 2px 0 rgba(0, 0, 0, .24));
  background-color: var(--timelineCardBackgroundColor, #fff);
}

/*
extensions
*/

.card__title{
  --rTitleMarginTop: var(--cardTitleMarginTop, 1rem);
  font-size: var(--cardTitleFontSize, 1.25rem);
}

/*
=====
CORE STYLES
=====
*/

.timeline{
  display: var(--timelineDisplay, grid);
  grid-row-gap: var(--timelineGroupsGap, 2rem);
}

/*
1. If timeline__year isn't displaed the gap between it and timeline__cards isn't displayed too
*/

.timeline__year{
  margin-bottom: 1.25rem; /* 1 */
}

.timeline__cards{
  display: var(--timeloneCardsDisplay, grid);
  grid-row-gap: var(--timeloneCardsGap, 1.5rem);
}


/*
=====
SKIN
=====
*/

.timeline{
  --uiTimelineMainColor: var(--timelineMainColor, #222);
  --uiTimelineSecondaryColor: var(--timelineSecondaryColor, #fff);

  border-left: var(--timelineLineWidth, 3px) solid var(--timelineLineBackgroundColor, var(--uiTimelineMainColor));
  padding-top: 1rem;
  padding-bottom: 1.5rem;
}

.timeline__year{
  --timePadding: var(--timelineYearPadding, .5rem 1.5rem);
  --timeColor: var(--uiTimelineSecondaryColor);
  --timeBackgroundColor: var(--uiTimelineMainColor);
  --timeFontWeight: var(--timelineYearFontWeight, 400);
}

.timeline__card{
  position: relative;
  margin-left: var(--timelineCardLineGap, 1rem);
}

/*
1. Stoping cut box shadow
*/

.timeline__cards{
  overflow: hidden;
  padding-top: .25rem; /* 1 */
  padding-bottom: .25rem; /* 1 */
}

.timeline__card::before{
  content: "";
  width: 100%;
  height: var(--timelineCardLineWidth, 2px);
  background-color: var(--timelineCardLineBackgroundColor, var(--uiTimelineMainColor));

  position: absolute;
  top: var(--timelineCardLineTop, 1rem);
  left: -50%;
  z-index: -1;
}

/*
=====
SETTINGS
=====
*/
/**/
.timeline{
  --timelineMainColor: #1d1d1d;
}

/*
=====
DEMO
=====
*/

body{
  font-family: -apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Open Sans, Ubuntu, Fira Sans, Helvetica Neue, sans-serif;
  color: #222;

  background-color: #f0f0f0;
  margin: 0;
  display: flex;
  flex-direction: column;
}

p{
  margin-top: 0;
  margin-bottom: 1rem;
  line-height: 1.5;
  font-size: 20px;
}

p:last-child{
  margin-bottom: 0;
}

.page{
  max-width: 47rem;
  padding: 5rem 2rem 3rem;
  margin-left: auto;
  margin-right: auto;
}


.substack{
  border:1px solid #EEE; 
  background-color: #fff;
  width: 100%;
  max-width: 480px;
  height: 280px;
  margin: 1rem auto;;
}


.CV{
  display: flex;
  justify-content: flex-end;
  padding: 2rem;
  text-align: center;
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



  </style>
  