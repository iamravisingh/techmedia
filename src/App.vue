<template>
  <div>
  <div id="app">
    <div class = "container">
      <nav class="navbar is-fixed-top" role="navigation" aria-label="main navigation">
        <div class="navbar-brand">
          <div class="navbar-item">
            <h1>techmedia</h1>
          </div>

          <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
            <span aria-hidden="true"></span>
          </a>
        </div>

        <div id="navbarBasicExample" class="navbar-menu">
          <div class="navbar-end">
            <div class="navbar-item">
              <div class="buttons">
                <span>Attend</span>
                <span >Sponsor</span>
                <span>Get Involved</span>
                <span >Media</span>
                <span>Our Story</span>
                <span>Subscribe</span>
              </div>
            </div>
          </div>
        </div>
      </nav>
      
    </div>
  </div>
  <div>
      <img src = "../src/assets/02_Header_Banner_Background image.png">
      <div class = "imageCaption">"Being and entrepreneur is a marathorn,it is not a point"</div>
  </div>
  <div class = "container">
    <div class = "columns">
      <section class="hero column is-three-quarters" id = "mainColumn">
        <div class="hero-body">
          <div class="container">
            <div class = "start">
            <span class = "first">CHICAGO</span>&nbsp;&nbsp;
            <span class = "second">FOUNDER FEATURE</span>
            </div>
            <br/>
            <h1 class="title">
              if you don't know your customer,you're barking up the wrong tree
            </h1>
            <span class = "date">BY TECHWEEK HQ | SEPTEMBER 5,2017, 3:14 PM CDT | 5 MIN READ</span>
          </div>
        </div>
      <section class="column is-icon-mobile">
        <span class = "icon"><img src = "../src/assets/Facebook.svg"></span>
        <span class = "icon"><img src = "../src/assets/Twitter.svg"></span>
        <span class = "icon"><img src = "../src/assets/Linkedin.svg"></span>
      </section>
      <div class = "columns">
         <div class = "column is-one-fifth is-mobile">
              <figure class="image is-64x64">
                <img class="is-rounded" src="../src/assets/04_Kristi Profile image.png">
              </figure>
           <div class = "mobileTitle">
              <strong>KRISTI ZUKHLE</strong>
              <br/>
              <span>Founder, knowledgeHound | Contributor</span>
           </div>
        </div>
        <div class = "column is-one-fifth is-desktop">
            <figure class="image is-64x64">
              <img class="is-rounded" src="../src/assets/04_Kristi Profile image.png">
            </figure>
            <br/>
            <strong>KRISTI ZUKHLE</strong>
            <br/>
            <span>Founder, knowledgeHound</span>
            <br/>
            <span>CONTRIBUTOR</span>
            <hr/>
            <strong>Company Overview</strong>
            <br/><br/>
            <strong>Website:</strong><br/>
            <span>www.knowledgeHound.com</span>
            <br/><br/>
            <strong>Industry:</strong><br/>
            <span>B2B SaaS Security</span>
            <br/><br/>
            <strong>Number of employees:</strong><br/>
            <span>OB</span>
            <br/><br/>
            <strong>Amount raised:</strong><br/>
            <span>$700000</span>
            <br/><br/>
            <strong>HQ location:</strong><br/>
            <span>chicago</span>
            <br/><br/>
            <strong>Fact:</strong><br/>
            <span>10,000 email sent</span>
        </div>
        <div class = "column is-two-thirds">
          <p><strong>CHICAGO:</strong> Consumer packaged good (CPG) companies have massive
          market budget we know this -- think of olympics P&G commercial
          that aired.But do you know at average 47% of their marketing budgets
          are spent on marketing research and yet today there are few tools to
          seach, categorize, and sift through all those report? Think how frustating
          it would be spend figures on a report and then not be able to recall it?</p><br/>
          <img src = "../src/assets/05_Blog_Image1.png">
          <span class = "imageTitle">Lorem ipsum dolor sit amet, consectetur adipiscing elit </span>
          <br/><br/>
          <p>In step Kristi zulke,Founder of knowledgeHound, a young chicago startup
            building software for fortune 500 compaines to manage these repors
            seemlessly.Not only does she have a great product but she's built a great 
            team a value and culture that is truly inspring.Techweek CEO, Amanda
            Signorelli, sat down with kristi to learn more.
          </p>
          <br/><br/><br/>
        </div>
      </div>
      </section>
      <section class="hero column is-desktop">
        <div class="hero-body">
          <rightComponent></rightComponent>
        </div>
      </section>
    </div>
    <subSection></subSection>
    <br/><br/><br/>
    <recommendation></recommendation>
    <br/><br/><br/>
    <footerSection></footerSection>
  </div>
  </div>
</template>

<script>
import subSection from '../src/component/subsection';
import recommendation from '../src/component/recommendation';
import footerSection from '../src/component/footer';
import rightComponent from '../src/component/rightComponent';

export default {
  name: 'app',
  data () {
    return {

    }
  },
  components : {
    subSection,
    recommendation,
    footerSection,
    rightComponent
  }
}
</script>

<style lang="scss" src="bulma"></style>
<style lang="css">
@import './css/animation.css';
  #app{
      background-color: #ff4838;
      color : white
  }

  span{
    color: grey;
  }

  .container > nav{
    background-color: #ff4838;
    color : white
  }

  .navbar-end{
    margin : 0 auto;
    text-align: center;
  }

  .buttons > span{
    padding: 10px;
    color: white;
  }

  .navbar-brand > .navbar-item > h1{
    color : white;
    font-size: x-large;
  }

  .is-one-fifth{
    font-size: 12px;
  }

  .date{
      font-size: 10px;
  }

@media only screen and (max-width: 768px){
  .is-mobile{
    border-top: 1px solid #cecaca;
    border-bottom: 1px solid #cecaca;
    display: flex;
    margin: 0 20px 0 20px;
  }
  .mobileTitle{
        margin: 14px 0 0 12px;
  }
}

@media only screen and (min-width: 769px){
  .is-mobile,.is-icon-mobile{
        display: none;
  }


}
@media only screen and (max-width: 768px){
  .is-desktop{
    display: none;
  }

  #mainColumn > .hero-body{
    padding-bottom: 0;
  }

  .is-icon-mobile{
    padding : 17px 0px 17px 16px;
  }
  
  .is-icon-mobile > span{
    width: 61px;
    height: 16px;

  }

  .is-two-thirds{
    margin : 0 20px 0 20px;
  }
}
  .imageTitle{
        font-size: 13px;

  }

.involved{
  font-size: 13px;
} 

.involved > div{
  border : 1px solid;
}

.involveSubSection{
      font-size: 12px;
}

.start{
  font-size: 9px;
}

.start > span{
  color: #ff4838;
}

.start > .second{
    background: #ff4838;
    color: white;
    padding: 4px;
}
.start > .first{
  border: 1px solid #ff4838;
  padding: 3px 4px 3px 4px;
}

@media screen and (min-width: 1024px){
  .navbar-brand{
        margin-left: 4rem !important;
  }
}
.imageCaption{
  position: absolute;
  top: 99px;
  left: 28rem;
  color: white;
}

</style>

