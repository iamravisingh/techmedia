<template>
  <div class = "container">
      <strong>Recommendation</strong>
      <hr/>
      <br/><br/>
    <div>
        <div class="slideshow-container">

            <div class="mySlides fade">
            <div class="numbertext">1 / 3</div>
            <img src="../assets/Image_1.png" style="width:100%">
            <div class="text">Caption Text</div>
            </div>

            <div class="mySlides fade">
            <div class="numbertext">2 / 3</div>
            <img src="../assets/image_2.png" style="width:100%">
            <div class="text">Caption Two</div>
            </div>

            <div class="mySlides fade">
            <div class="numbertext">3 / 3</div>
            <img src="../assets/image_3.png" style="width:100%">
            <div class="text">Caption Three</div>
            </div>

            </div>
            <br>

            <div style="text-align:center">
            <span class="dot" @click = showSlides></span> 
            <span class="dot" @click = showSlides></span> 
            <span class="dot" @click = showSlides></span> 
            </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'Test',
    data(){
        return {
            test : ''
        }
    },
    mounted(){
        console.log('hi there mounted >>>>>>>>>>>>>>>>');
        this.showSlides();
        // this.init()
    },
    methods: {
        showSlides(){
            var i; 
            var slideIndex = 0;
            // get the array of divs' with classname image-sliderfade 
            var slides = document.getElementsByClassName("mySlides"); 
            
            // get the array of divs' with classname dot 
            var dots = document.getElementsByClassName("dot"); 

            for (i = 0; i < slides.length; i++) { 
                // initially set the display to 
                // none for every image. 
                slides[i].style.display = "none"; 
            } 

            // increase by 1, Global variable 
            slideIndex++; 

            // check for boundary 
            if (slideIndex > slides.length) 
            { 
                slideIndex = 1; 
            } 

            for (i = 0; i < dots.length; i++) { 
                dots[i].className = dots[i].className. 
                                    replace(" active", ""); 
            } 

            slides[slideIndex - 1].style.display = "block"; 
            dots[slideIndex - 1].className += " active"; 

            // Change image every 2 seconds 
            // setTimeout(this.showSlides, 2000); 
        }
    }
}
</script>

<style scoped> 
@import '../css/slider.css';
.container{
    margin: 0 139px 0 139px;
}

@media only screen and (max-width: 768px){
.container{
    margin: 0 20px 0 20px;
}
}


</style>