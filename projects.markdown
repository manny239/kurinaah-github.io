---
layout: page
title: "Projects"
permalink: /projects/
---

# Projects

Here are some projects that I have completed and some that I am still working on:

**Automated Parking Monitoring System**: <br>
I am currently working on this project as a Senior Capstone Design Project. This project was designed to ease parking on the University of Hartford campus by providing occupancy status on each single parking space within a parking lot using Machine Learning and Real Time Streaming Protocol (RTSP) enabled cameras connected to a Raspberry pi 5 Microcontroller. <br>
A schematic of the parking lot is designed and shown to users on a website created through REACT. Occupied parking spaces are denoted with a red box and empty spaces denoted with a green box to help students know exactly where to park and which parking lots have spots open at any given point in time. This can be extended for bigger parking lots and has several advantages over systems that use IoT sensors as the cameras used in this project have a good field of view that allows a greater coverage with less components. 
For going green and smart city initiatives, this can be an important cog in the machine!<br>
[Link to Publication](https://spie.org/defense-commercial-sensing/presentation/Real-time-parking-lot-monitoring-for-smart-cities--a/13465-61)


<!-- Carousel container -->
<div class = "carousel" >
    <img src="/assets/images/image1.jpg" alt="Pic1" class="active"/>
    <img src="/assets/images/image2.png" alt ="Pic2" />
    <img src="/assets/images/image3.jpg" alt ="Pic3" />
    <img src="/assets/images/image4.jpg" alt ="Pic4" />
</div>

<!-- Button to play/pause picture -->
<button id="carousel-button" onclick="togglePause()"> Pause </button>

<!-- Inlines CSS for styling the carousel -->
<style>
.carousel{
    width: 700px;
    height: 400px;
    position: relative;
    margin-bottom: 1rem;
}
.carousel img{
    position: absolute;
    display: none;
    width: 100%;
    height: 100%;
    object-fit: cover;
}
.carousel img.active{
    display: block;
}
#carousel-button {
    display: block;
    margin: 0 auto;
    background-color: #d9ce15;
}
</style>

<!-- Inline js code to create carousel cycling -->
<script> 
    const images = document.querySelectorAll('.carousel img')
    let currentIndex = 0;
    let isPaused = false;
    const displayInterval = 3000;
    const button = document.getElementById('carousel-button');

    //Auto advance every display interval
    let interval = setInterval(nextImage, displayInterval);

    function nextImage() {
        if (isPaused) return;
        images[currentIndex].classList.remove('active');
        currentIndex = (currentIndex + 1) % images.length;
        images[currentIndex].classList.add('active');
    }

    function togglePause() {
        isPaused = !isPaused;
        button.textContent = isPaused ? 'Play' : 'Pause';
    }
</script>

**Tennis Court Reservation & Management Website**: This is a semester long project for a CS460: Software Development class. This class covers product development using both the Agile and Scrum development methodologies. The goal of the project was to develop a fully-function web application to manage operations such as new account creation, member login, court reservation and many other functionalities for a tennis club. <br>
<t> As-Is-Product (Still in development)

<!-- Video import container -->
<div class = "video">
    <video src="/assets/videos/video1.mp4" autoplay loop muted playsinline> </video>
</div>

<div class="video-controls" style="text-align: center; margin-top: 1rem; ">
    <span id="fullscreen-icon" onclick="openFullscreen()" style="cursor:pointer; font-size: 24px; margin-right:10px; " > ⛶ </span>
    <span id="minimize-icon" onclick="closeFullscreen()" style="cursor:pointer; font-size: 24px; "> 🗗 </span>
</div>

<!-- Styling for video -->
<style>
.video {
    width: 700px;
    height: 400px;
    position: relative;
    margin-bottom: 1rem;
}
.video video {
    width: 100%;
    height: 100%
    object-fit: contain;
}
</style>

<!-- JS for fullscreen and minimize functionality-->
<script> 
    var videoContainer = document.querySelector('.video')

    function openFullscreen() {
        if (videoContainer.requestFullscreen) {
            videoContainer.requestFullscreen();
        }
        else if (videoContainer.mozRequestFullScreen) { /* Firefox */
            videoContainer.mozRequestFullScreen();
        }
        else if (videoContainer.webkitRequestFullscreen) { /* Chrome, Safari, Opera */
            videoContainer.webkitRequestFullscreen();
        }
        else if (videoContainer.msRequestFullscreen) { /* MS Edge */
            videoContainer.msRequestFullscreen();
        }
    }

    function closeFullscreen() {
        if (document.exitFullscreen) {
            document.exitFullscreen();
        }
        else if (document.mozCancelFullScreen) { /* Firefox */
            document.mozCancelFullScreen();
        } 
        else if (document.webkitExitFullscreen) { /* Chrome, Safari and Opera */
            document.webkitExitFullscreen();
        } 
        else if (document.msExitFullscreen) { /* IE/Edge */
            document.msExitFullscreen();
        }
    }
</script>

<br>
Speed Checker Design :
This project is partenered and sponsored by the Public Safety department here at the University of Hartford. More information will be provided soon on this platform. <br>

<br>
Travel Itinerary WebApp: Design of a web application that uses API calls to provide a personalized itinerary from chatGPT Model 3.5. More information will be uploaded soon.<br>

<br>
Vehicle Guidance System: More information on this project will be provided soon



