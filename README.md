<div id="profile-container" style="position: relative; background-color: #1a1a1a; color: #ffffff; padding: 20px; border-radius: 10px; overflow: hidden;">

  <!-- Animated Background -->
  <div id="animated-bg" style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; overflow: hidden;">
    <img src="background-image.jpg" alt="Animated Background" style="width: 100%; height: 100%; object-fit: cover; filter: brightness(70%);">
  </div>

  <!-- Profile Image -->
  <img src="your_profile_image_url.jpg" alt="Profile Image" style="border-radius: 50%; width: 150px; height: 150px; position: relative; z-index: 1;">

  <!-- Introduction -->
  <h1>Hello, I'm [Your Name]</h1>
  <p>🚀 Aspiring Integrated MCA | Passionate about coding, problem-solving, and learning new technologies.</p>

  <!-- Tech Stack -->
  <h2>🛠️ Tech Stack</h2>
  <p>HTML | CSS | Python | C | C++ | DSA | DBMS</p>

  <!-- Social Profiles with Icons -->
  <h2>🌐 Social Profiles</h2>
  <a href="https://twitter.com/your_twitter" target="_blank"><img src="twitter-icon.png" alt="Twitter Icon" style="width: 30px; height: 30px;"></a>
  <a href="https://instagram.com/your_instagram" target="_blank"><img src="instagram-icon.png" alt="Instagram Icon" style="width: 30px; height: 30px;"></a>
  <a href="https://t.me/your_telegram" target="_blank"><img src="telegram-icon.png" alt="Telegram Icon" style="width: 30px; height: 30px;"></a>

  <!-- Professional Profiles with Icons -->
  <h2>👔 Professional Profiles</h2>
  <a href="https://linkedin.com/in/your_linkedin" target="_blank"><img src="linkedin-icon.png" alt="LinkedIn Icon" style="width: 30px; height: 30px;"></a>
  <a href="https://github.com/your_github" target="_blank"><img src="github-icon.png" alt="GitHub Icon" style="width: 30px; height: 30px;"></a>
  <a href="https://www.codingninjas.com/profiles/your_codingninjas" target="_blank"><img src="codingninjas-icon.png" alt="Coding Ninjas Icon" style="width: 30px; height: 30px;"></a>
  <!-- Add similar lines for other professional profiles -->

  <!-- Campus Ambassador Roles -->
  <h2>🎓 Campus Ambassador</h2>
  <p>GeeksforGeeks | Zuno (Leadership Skills)</p>

  <!-- Hobbies and Activities -->
  <h2>🌟 Hobbies and Activities</h2>
  <p>🔍 Interact, play CTF challenges, blogging, learn new things</p>

  <!-- Websites -->
  <h2>🌐 Websites</h2>
  <a href="https://ip1jnvkarauli.blogspot.com" target="_blank">ip1jnvkarauli.blogspot.com</a>

  <!-- Volunteer Work -->
  <h2>🤝 Volunteer Work</h2>
  <p>Google Map | Google CloudSource</p>

  <!-- Add JavaScript for Background Animation -->
  <script>
    const animatedBg = document.getElementById('animated-bg');
    let offsetX = 0;
    let offsetY = 0;

    function moveBackground(event) {
      offsetX = -event.clientX / 10;
      offsetY = -event.clientY / 10;
      animatedBg.style.transform = `translate(${offsetX}px, ${offsetY}px)`;
    }

    document.addEventListener('mousemove', moveBackground);
  </script>

</div>


<style>
  @color: #5bc0eb;

* {
    box-sizing: border-box;
}


@keyframes move-dot1 {
    0% {
        transform: translateX(-50%) translateY(-50%);
    }
    
    20% {
        transform: translateX(-50%) translateY(30%);
    }
    
    100% { 
        transform: translateX(-50%) translateY(30%);
    }
}


@keyframes move-dot2 {
    0% {
        transform: translateX(-50%) translateY(-50%);
    }
    
    15% {
        transform: translateX(-50%) translateY(-10%);
    }
    
    30% {
        transform: translateX(-10%) translateY(-10%);
    }
    
    100% { 
        transform: translateX(-10%) translateY(-10%);
    }
}


body {
    background: #000;
}


.animation-example {
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translateX(-50%) translateY(-50%);
    height: 90vmin;
    width: 90vmin;
    
    > .item {
        position: absolute;
        top: 0;
        left: 50%;
        height: 50%;
        width: 50%;
        transform: translateX(-50%);
        transform-origin: 50% 100%;
        pointer-events: none;
    }
    
    > .item:nth-child(2) {
        transform: translateX(-50%) rotate(90deg);
    }
    
    > .item:nth-child(3) {
        transform: translateX(-50%) rotate(180deg);
    }
    
    > .item:nth-child(4) {
        transform: translateX(-50%) rotate(270deg);
    }
    
    > .item > .line {
        height: 100%;
        width: ~"calc(50% + 1px)";
        border-right: 2px dashed @color;
    }
    
    > .item > .dot {
        position: absolute;
        left: 50%;
        top: 10%;
        transform: translateX(-50%) translateY(-50%);
        height: 100%;
        width: 100%;
        animation: move-dot1 5.5s linear infinite;
    }
    
    > .item > .dot::after {
        content: '';
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translateX(-50%) translateY(-50%);
        height: 5%;
        width: 5%;
        background: #fff;
        border: 2px solid @color;
        border-radius: 50%;
    }

    > .item > .circle {
        position: absolute;
        top: 0;
        left: 50%;
        transform: translateX(-50%);
        height: 20%;
        width: 20%;
        border-radius: 50%;
        background: @color;
    }
    
    > .item.-type2 {
        top: 0;
        left: 0;
        transform: none;
        transform-origin: 100% 100%;
    }
    
    > .item.-type2:nth-child(5) {
        transform: scaleX(-100%);
    }
    
    > .item.-type2:nth-child(6) {
        transform: scaleX(-100%) scaleY(-100%);
    }
    
    > .item.-type2:nth-child(7) {
        transform: scaleY(-100%);
    }
    
    > .item.-type2 > .line {
        position: absolute;
        top: 30%;
        left: ~"calc(30% - 1px)";
        width: 70%;
        height: 40%;
        border-right: none;
        border-left: 2px dashed @color;
        border-bottom: 2px dashed @color;
    }
    
    > .item.-type2 > .dot {
        top: 30%;
        left: 30%;
        animation: move-dot2 4s linear infinite;
    }
    
    > .item.-type2 > .circle {
        top: 30%;
        left: 30%;
        transform: translateX(-50%) translateY(-50%);
    }
    
    > .item:nth-of-type(1) > .dot {
        animation-delay: 0;
    }
    
    > .item:nth-of-type(7) > .dot {
        animation-delay: .5s;
    }
    
    > .item:nth-of-type(2) > .dot {
        animation-delay: 1s;
    }
    
    > .item:nth-of-type(6) > .dot {
        animation-delay: 1.5s;
    }
    
    > .item:nth-of-type(3) > .dot {
        animation-delay: 2s;
    }
    
    > .item:nth-of-type(5) > .dot {
        animation-delay: 2.5s;
    }
    
    > .item:nth-of-type(4) > .dot {
        animation-delay: 3s;
    }
    
    > .item:nth-of-type(8) > .dot {
        animation-delay: 3.5s;
    }
    
    > .center {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translateX(-50%) translateY(-50%);
        height: 50%;
        width: 50%;
    }
    
    > .center > .circle {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translateX(-50%) translateY(-50%);
        border-radius: 50%;
    }
    
    > .center > .circle:nth-child(1) {
        height: 100%;
        width: 100%;
        background: #fff;
        box-shadow: 0 0 3vmin rgba(0, 0, 0, .1);
    }
    
    > .center > .circle:nth-child(2) {
        height: 80%;
        width: 80%;
        border: 2px solid @color;
    }
    
    > .center > .circle:nth-child(3) {
        height: 50%;
        width: 50%;
        background: @color;
    }
}

</style>
<div class='animation-example'>
    <div class='item'>
        <div class='line'></div>
        <div class='dot'></div>
        <div class='circle'></div>
    </div>
    <div class='item'>
        <div class='line'></div>
        <div class='dot'></div>
        <div class='circle'></div>
    </div>
    <div class='item'>
        <div class='line'></div>
        <div class='dot'></div>
        <div class='circle'></div>
    </div>
    <div class='item'>
        <div class='line'></div>
        <div class='dot'></div>
        <div class='circle'></div>
    </div>
    <div class='item -type2'>
        <div class='line'></div>
        <div class='dot'></div>
        <div class='circle'></div>
    </div>
    <div class='item -type2'>
        <div class='line'></div>
        <div class='dot'></div>
        <div class='circle'></div>
    </div>
    <div class='item -type2'>
        <div class='line'></div>
        <div class='dot'></div>
        <div class='circle'></div>
    </div>
    <div class='item -type2'>
        <div class='line'></div>
        <div class='dot'></div>
        <div class='circle'></div>
    </div>
    <div class='center'>
        <div class='circle'></div>
        <div class='circle'></div>
        <div class='circle'></div>
    </div>
</div>
