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
