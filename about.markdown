---
layout: page
title: About
permalink: /about/
---

<div class="hobbies-list"> 
    <ul> 
        <li> Innovator 🧠 </li>
        <li> Fullstack Application Developer 💼 </li>
        <li> AI & Machine Learning Enthusiast 🤖 </li>
        <li> Leader & Team Player 💪 </li>
        <li> Public Speaker 🎤  </li>
        <li> Athlete 🏆 </li>
    </ul>
</div>

<div class="hobbies"> 
    <img src="/assets/images/ball.JPG" alt="basketball-photo">
    <img src="/assets/images/speak.JPEG" alt="public-speaking">
    <img src="/assets/images/soccer.JPG" alt="soccer-photo">
</div>

<style>
.hobbies-list {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
}

.hobbies {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
}

/* Style for the first two images */
.hobbies img {
    width: calc(50% - 5px);
}

/* Make the third image span the full row */
.hobbies img:nth-child(3) {
    width: 100%
}
</style>
