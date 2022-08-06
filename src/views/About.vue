<template>
    <main class="about-page">
        <header class="container">
            <h1>Welcome to my About page.</h1>
            <h2>Scroll down to see more information<p class="animate-arrow">&darr;</p></h2>
        </header>
        <section class="containter">
            
            <div class="about-container">
                <div class="photos">
                    <div class="box">
                        <img src="../assets/marine1.jpg"  class="image-about">
                    </div>
                    <div class="box">
                        <img src="../assets/marine2.jpg" class="image-about">
                    </div>
                    <div class="box">
                        <img src="../assets/marine3.jpg"  class="image-about">
                    </div>
                    <div class="box">
                        <img src="../assets/marine4.jpg"  class="image-about">
                    </div>
                    <div class="box">
                        <img src="../assets/marine5.jpg"  class="image-about">
                    </div>
                    <div class="box">
                        <img src="../assets/marine6.jpg"  class="image-about">
                    </div>
                    <div class="box">
                        <img src="../assets/marine7.jpg"  class="image-about">
                    </div>
                    <div class="box">
                        <img src="../assets/marine8.jpg"  class="image-about">
                    </div>
                    <div class="box">
                        <img src="../assets/marine9.jpg"  class="image-about">
                    </div>
                </div>
                <div class="text">
                <h3>Marine Corps Days</h3>
                <p>
                   I enlisted in the military when I was 23. At this point in my life I was just finishing up my undergrad in music performance and chose the military because throughout my undergrad I did not have any real direction to where I wanted to take my musical abilities. On January 4th of 2015 I shipped out to Marine Corps Recruit Depot San Diego for basic training. Training in the marine corps lasted until November of 2015 and that included basic training, combat training, and the Navy School of Music. From Novemeber of 2015 to January 2019 I was stationed at Marine Corps Base Kaneohe Bay, Oahu.  
                </p>
                </div>
            </div>
            
        </section>

        <section class="containter">
            <div class="about-container">
                <div class="text">
                    <h3>College all over again</h3>
                    <p>
                        The military provides all veterans with the GI bill. The benefits of this bill vary based on how long you are in but it does guarantee every service member with 36 months of paid tuition to any University. As my time in the military came to a close I decided to go back to school to persue a Master’s Degree in Music Industry Leadership at Northeastern University. This program lasted one and a half years and I was able to meet some amazing people I am still close with today. I graduated in April of 2020, a pretty turmoil period of time. The music industry had largely shut its doors at the start of the pandemic and interviews I had set up fell through. It was time to find a new profession.       
                    </p>
                </div>
                        <div class="photos">
                        <div class="box">
                            <img src="../assets/college1.jpg"  class="image-about">
                        </div>
                        <div class="box">
                            <img src="../assets/college2.jpg" class="image-about">
                        </div>
                        <div class="box">
                            <img src="../assets/college3.jpg"  class="image-about">
                        </div>
                        <div class="box">
                            <img src="../assets/college4.jpg"  class="image-about">
                        </div>
                        <div class="box">
                            <img src="../assets/college5.jpg"  class="image-about">
                        </div>
                        <div class="box">
                            <img src="../assets/college6.jpg"  class="image-about">
                        </div>
                        <div class="box">
                            <img src="../assets/college7.jpg"  class="image-about">
                        </div>
                        <div class="box">
                            <img src="../assets/college8.jpg"  class="image-about">
                        </div>
                        <div class="box">
                            <img src="../assets/todo1.jpg"  class="image-about">
                        </div>
                    </div>
                </div>
        </section>
                <section class="containter">
            <div class="about-container">
                <div class="photos">
                    <div class="box">
                        <img src="../assets/cs1.jpg"  class="image-about">
                    </div>
                    <div class="box">
                        <img src="../assets/cs2.jpg" class="image-about">
                    </div>
                    <div class="box">
                        <img src="../assets/cs3.jpg"  class="image-about">
                    </div>
                    <div class="box">
                        <img src="../assets/cs4.jpg"  class="image-about">
                    </div>
                    <div class="box">
                        <img src="../assets/todo5.jpg"  class="image-about">
                    </div>
                    <div class="box">
                        <img src="../assets/todo6.jpg"  class="image-about">
                    </div>
                    <div class="box">
                        <img src="../assets/todo7.jpg"  class="image-about">
                    </div>
                    <div class="box">
                        <img src="../assets/todo8.jpg"  class="image-about">
                    </div>
                    <div class="box">
                        <img src="../assets/todo1.jpg"  class="image-about">
                    </div>
                </div>
                <div class="text">
                <h3>MA in CS</h3>
                <p>
                    I originally applied to my alma mater for there MA program in CS for individuals who didn’t come from a CS background. I unfortunately did not get in but it allowed me to find a new place of learning. Boston University! Like many student looking to receive a MA in CS with no background I had to complete four, 400 level courses with high marks. By Spring of 2021 I was in and my MA in CS at Boston University began.  I have enjoyed the MA Computer Science program at BU so far and definitely ready to get out in to the field when my time at BU comes to an end. I have always enjoyed designing and arranging rooms to best fit the space available and would like to somehow find how that pasion can relate to a job within the programming job market. Maybe something with UI design or an area of system architecture. I enjoy playing music in my free time, gaming, and like many, being outside in nature as much as possible.     
                </p>
                </div>
            </div>
        </section>
    </main>
</template>

<script>



</script>

<style>
body {
    font-family: 'Fira sans', sans-serif;
    background: #4158D0;
    background: linear-gradient(
    115deg,
    rgba(86, 216, 228, 1) 10% ,
    rgba(159, 1, 234, 1) 90%);
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}

header {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    font-family: "Merriweather", serif;
    height: 100vh;
}

header h2 {
    font-weight: 400;
}

.about-page {
       animation: fadeInAnimation ease .5s;
            animation-iteration-count: 1;
            animation-fill-mode: forwards;
        }
        @keyframes fadeInAnimation {
            0% {
                opacity: 0;
            }
            100% {
                opacity: 1;
            }
}
 
.container {
    max-width: 1280px;
    width: 95%;
    margin: 0 auto;
}

.about-container {
    display: flex;
    align-items: center;
    height: 100vh;
}

.text {
    margin-left: 1rem;
    line-height: 2.5rem;  
}

.photos {
    display: grid;
    grid-template-rows: 300px 300px 300px;
    grid-template-columns: 300px 300px 300px;
}

.box {
    background: none;
    display: flex;
    align-items: center;
    justify-content: center;
    color: #AAA;
}

.image-about {
    width: 300px;
    height: 300px;
    object-fit: cover;
    padding: 5px;
    border-radius: 1.2rem;
    box-shadow: 2px 2px 2px; 
    cursor: pointer; 
    -webkit-transition-property: all; 
    -webkit-transition-duration: 0.3s; 
    -webkit-transition-timing-function: ease;  
}

.image-about:hover {
    transform: scale(1.2);
}

@media screen and (max-width: 1380px)  {    
    .photos { display: none; } 
}

</style>