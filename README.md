<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
  <title>Mohit Jani — Robotics Engineer | Portfolio</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif;
      background: #fafafc;
      color: #1e1e2f;
      line-height: 1.55;
      scroll-behavior: smooth;
    }

    .container {
      max-width: 1100px;
      margin: 0 auto;
      padding: 2rem 1.5rem;
    }

    /* Sticky nav bar with buttons */
    .nav-bar {
      position: sticky;
      top: 0;
      z-index: 100;
      background: rgba(255, 255, 255, 0.92);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid rgba(0, 0, 0, 0.05);
      padding: 0.85rem 1.5rem;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 0.75rem;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.02);
    }

    .nav-btn {
      background: transparent;
      border: none;
      font-size: 1rem;
      font-weight: 500;
      padding: 0.5rem 1.4rem;
      border-radius: 40px;
      cursor: pointer;
      transition: all 0.2s ease;
      font-family: inherit;
      color: #2c3e66;
      background: #f0f2f8;
    }

    .nav-btn:hover {
      background: #e0e4ed;
      transform: translateY(-1px);
    }

    .nav-btn:active {
      transform: translateY(1px);
    }

    /* hero header */
    .hero h1 {
      font-size: 2.8rem;
      letter-spacing: -0.02em;
      background: linear-gradient(135deg, #1e2b3c, #2a4b6e);
      background-clip: text;
      -webkit-background-clip: text;
      color: transparent;
      margin-bottom: 0.25rem;
    }

    .contact {
      font-size: 1.1rem;
      margin: 0.75rem 0 1rem;
    }

    hr {
      margin: 1.8rem 0;
      border: none;
      height: 1px;
      background: linear-gradient(90deg, #ddd, transparent);
    }

    .section {
      margin-bottom: 3rem;
      scroll-margin-top: 80px;
    }

    h2 {
      font-size: 1.9rem;
      font-weight: 600;
      letter-spacing: -0.3px;
      border-left: 5px solid #2a7f6e;
      padding-left: 1rem;
      margin-bottom: 1.5rem;
      color: #1a2c3c;
    }

    h3 {
      font-size: 1.4rem;
      font-weight: 600;
      margin: 1rem 0 0.25rem;
      color: #1f3b4c;
    }

    .job-title {
      font-weight: 600;
      color: #2a7f6e;
    }

    .date {
      color: #5b6e8c;
      font-size: 0.85rem;
      font-weight: normal;
      margin-left: 0.5rem;
    }

    ul {
      padding-left: 1.5rem;
      margin: 0.5rem 0 1rem;
    }

    li {
      margin: 0.5rem 0;
    }

    /* image & video gallery grids */
    .media-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 1.5rem;
      margin: 1.8rem 0 1rem;
    }

    .media-card {
      flex: 1 1 280px;
      background: #ffffff;
      border-radius: 20px;
      overflow: hidden;
      box-shadow: 0 8px 20px rgba(0,0,0,0.05);
      transition: transform 0.2s, box-shadow 0.2s;
      border: 1px solid #eef2f5;
    }

    .media-card:hover {
      transform: translateY(-4px);
      box-shadow: 0 16px 28px rgba(0,0,0,0.08);
    }

    .media-img {
      width: 100%;
      height: 180px;
      object-fit: cover;
      background: #eef2fa;
      display: block;
    }

    .video-wrapper {
      position: relative;
      width: 100%;
      background: #000;
    }

    .video-wrapper video {
      width: 100%;
      height: 180px;
      object-fit: cover;
      display: block;
    }

    .media-caption {
      padding: 0.8rem 1rem;
      font-size: 0.85rem;
      font-weight: 500;
      background: white;
      color: #2c3e66;
      border-top: 1px solid #eff3f8;
    }

    .placeholder-img {
      background: linear-gradient(145deg, #cddfe7, #b8cfdd);
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 2rem;
      color: #2a5f6e;
      height: 180px;
    }

    .skill-badge {
      display: inline-block;
      background: #eef2fa;
      padding: 0.2rem 0.7rem;
      border-radius: 20px;
      font-size: 0.8rem;
      margin-right: 0.5rem;
      margin-bottom: 0.5rem;
    }

    .contact-links {
      margin-top: 1rem;
      display: flex;
      gap: 1.5rem;
      flex-wrap: wrap;
    }

    .btn-outline {
      background: transparent;
      border: 1.5px solid #2a7f6e;
      padding: 0.5rem 1.2rem;
      border-radius: 30px;
      font-weight: 500;
      transition: 0.2s;
      display: inline-block;
      color: #2a7f6e;
      text-decoration: none;
    }

    .btn-outline:hover {
      background: #2a7f6e;
      color: white;
      border-color: #2a7f6e;
    }

    footer {
      margin-top: 3rem;
      text-align: center;
      font-size: 0.8rem;
      color: #6c7a8e;
      border-top: 1px solid #e2e8f0;
      padding-top: 2rem;
    }

    @media (max-width: 680px) {
      .container {
        padding: 1.2rem;
      }
      .hero h1 {
        font-size: 2rem;
      }
      h2 {
        font-size: 1.6rem;
      }
      .nav-btn {
        padding: 0.4rem 1rem;
        font-size: 0.85rem;
      }
    }
  </style>
</head>
<body>

<div class="nav-bar">
  <button class="nav-btn" data-section="about">📄 About</button>
  <button class="nav-btn" data-section="experience">💼 Experience</button>
  <button class="nav-btn" data-section="projects">⚙️ Projects</button>
  <button class="nav-btn" data-section="gallery">🖼️ Media</button>
  <button class="nav-btn" data-section="contact">📬 Contact</button>
</div>

<div class="container">
  <div class="hero" id="about">
    <h1>Mohit Jani</h1>
    <p class="contact">
      <a href="mailto:mohit10.jani@gmail.com">mohit10.jani@gmail.com</a> | +91 97375 06559 | Surat, India
    </p>
    <hr>
  </div>

  <!-- About section -->
  <div class="section" id="about-section">
    <h2>About</h2>
    <p>I am a <strong>Design & Development Engineer</strong> specializing in <strong>Robotics, Computer Vision, and Precision Assembly</strong>. I build systems that bridge the gap between digital models and real-world hardware with high reliability.</p>
    <p>Drawn to <strong>Neuralink</strong> and brain-computer interfaces because I believe in amplifying human capability through precise human-machine collaboration.</p>
    <!-- small image embedded in about to demo visual style -->
    <div class="media-grid" style="margin-top: 1.2rem;">
      <div class="media-card">
        <div class="placeholder-img" style="background: #d9e6f2;">
          🤖⚡
        </div>
        <div class="media-caption">Robotics lab — precision assembly testing</div>
      </div>
      <div class="media-card">
        <div class="placeholder-img" style="background: #cfe3e8;">
          🧠🔗
        </div>
        <div class="media-caption">BCI & human augmentation research</div>
      </div>
    </div>
  </div>

  <!-- Experience section -->
  <div class="section" id="experience-section">
    <h2>Experience</h2>
    <h3>Design & Development Engineer — Cynlr <span class="date">Feb 2024 – Present</span></h3>
    <ul>
      <li>Engineered stereo vision calibration system reducing convergence error from 10 mm to 3 mm — now company-wide standard.</li>
      <li>Developed force-compliant wire-insertion algorithm for Audi mirror assembly (5 mm clearance, 80% success in 2-min cycle); reused across projects.</li>
      <li>Built complete QA framework for 3-finger Tesello gripper (IK, grasping, control).</li>
      <li>Mastered LabVIEW mid-project for General Motors customer delivery.</li>
    </ul>

    <h3>Research Intern — Human Centered Robotics, IIT Gandhinagar <span class="date">May – Jul 2023</span></h3>
    <ul>
      <li>Simulated upper-limb musculoskeletal motion using MuJoCo + OpenAI Gym; data contributed to MyoSuite benchmarking tool.</li>
    </ul>
  </div>

  <!-- Selected projects section -->
  <div class="section" id="projects-section">
    <h2>Selected Projects</h2>
    <h3>Stereo Vision Convergence Improvement</h3>
    <p>Jul – Aug 2025 • Developed original geometric + vision models; validated on physical hardware.</p>

    <h3>Audi Mirror Wire Insertion (Force Compliance)</h3>
    <p>Sep 2025 – Mar 2026 • Achieved reliable insertion through tight clearance with full failure handling.</p>

    <h3>CanSat — ISRO / IN-SPACe Competition</h3>
    <p>2022 – 2024 • Full lifecycle aerospace project (concept to launch).</p>
  </div>

  <!-- MEDIA GALLERY: Images + Videos of projects (showcase) -->
  <div class="section" id="gallery-section">
    <h2>📸 Project Gallery & Demos</h2>
    <div class="media-grid">
      <!-- Image Card 1: Stereo Calibration rig -->
      <div class="media-card">
        <img class="media-img" src="https://placehold.co/600x400/2c5f6e/white?text=Stereo+Calibration+Rig" alt="Stereo vision prototype" loading="lazy">
        <div class="media-caption">🔍 Stereo vision calibration rig — 3mm convergence error achieved</div>
      </div>
      <!-- Image Card 2: Force compliant gripper -->
      <div class="media-card">
        <img class="media-img" src="https://placehold.co/600x400/3a6b5e/white?text=Force+Compliant+Gripper" alt="Force compliant assembly">
        <div class="media-caption">🦾 Force-compliant wire insertion (Audi mirror assembly)</div>
      </div>
      <!-- Image Card 3: CanSat Aerospace -->
      <div class="media-card">
        <img class="media-img" src="https://placehold.co/600x400/4a6c7c/white?text=CanSat+Launch+ISRO" alt="CanSat competition">
        <div class="media-caption">🚀 CanSat — ISRO/IN-SPACe, full aerospace lifecycle</div>
      </div>
    </div>

    <h3 style="margin-top: 1.2rem;">🎥 Demo Videos (Project in action)</h3>
    <div class="media-grid">
      <!-- Video 1: Stereo vision demo (local placeholder mp4 simulation / or embedded sample) 
           Using a sample webm from online asset + also fallback. For true demo we use loop muted autoplay? but user control better -->
      <div class="media-card">
        <div class="video-wrapper">
          <video controls preload="metadata" poster="https://placehold.co/600x400/2c3e50/white?text=Stereo+Vision+Demo">
            <source src="https://commondatastorage.googleapis.com/gtv-videos-bucket/sample/ForBiggerBlazes.mp4" type="video/mp4">
            Your browser does not support the video tag.
          </video>
        </div>
        <div class="media-caption">🎥 Stereo Vision calibration & real-time depth map</div>
      </div>
      <!-- Video 2: Force compliant insertion (realistic demo) -->
      <div class="media-card">
        <div class="video-wrapper">
          <video controls preload="metadata" poster="https://placehold.co/600x400/2c5f4a/white?text=Force+Insertion+Demo">
            <source src="https://commondatastorage.googleapis.com/gtv-videos-bucket/sample/ForBiggerEscapes.mp4" type="video/mp4">
          </video>
        </div>
        <div class="media-caption">⚙️ Force-compliant algorithm — Audi mirror assembly (tight clearance)</div>
      </div>
      <!-- Video 3: Tesello gripper QA + IK simulation -->
      <div class="media-card">
        <div class="video-wrapper">
          <video controls preload="metadata" poster="https://placehold.co/600x400/3c6e5e/white?text=Tesello+Gripper+Test">
            <source src="https://commondatastorage.googleapis.com/gtv-videos-bucket/sample/WhatCar.mp4" type="video/mp4">
          </video>
        </div>
        <div class="media-caption">🤖 Tesello 3-finger gripper — inverse kinematics & grasping suite</div>
      </div>
    </div>

    <!-- Additional custom images (optional for Cansat real) -->
    <div class="media-grid">
      <div class="media-card">
        <img class="media-img" src="https://placehold.co/600x400/287b6e/white?text=MuJoCo+Simulation" alt="MuJoCo simulation">
        <div class="media-caption">🧠 Upper-limb musculoskeletal simulation (IIT Gandhinagar)</div>
      </div>
      <div class="media-card">
        <img class="media-img" src="https://placehold.co/600x400/4f7a5b/white?text=LabVIEW+GM+Delivery" alt="LabVIEW control">
        <div class="media-caption">📊 LabVIEW automation framework for General Motors</div>
      </div>
    </div>
  </div>

  <!-- Education + Skills combined for clean view -->
  <div class="section">
    <h2>Education</h2>
    <p><strong>B.Tech Mechanical Engineering</strong><br>NIT Surat (SVNIT) — GPA 8.1/10 (2024)</p>
  </div>

  <div class="section">
    <h2>Technical Skills</h2>
    <p>
      <span class="skill-badge">Python</span> <span class="skill-badge">C/C++</span> <span class="skill-badge">LabVIEW</span> <span class="skill-badge">MATLAB</span>
      <span class="skill-badge">Inverse Kinematics</span> <span class="skill-badge">Robotic Grasping</span> <span class="skill-badge">Force Compliance</span>
      <span class="skill-badge">FANUC</span> <span class="skill-badge">Schunk</span> <span class="skill-badge">Stereo Calibration</span>
      <span class="skill-badge">SolidWorks</span> <span class="skill-badge">ANSYS</span> <span class="skill-badge">MuJoCo</span> <span class="skill-badge">OpenAI Gym</span>
      <span class="skill-badge">Arduino</span>
    </p>
  </div>

  <!-- Contact section with extra links + embedded call -->
  <div class="section" id="contact-section">
    <h2>Let’s Connect</h2>
    <p>Feel free to reach out — I'm always excited to discuss robotics, precision systems, or brain-computer interface applications.</p>
    <div class="contact-links">
      <a href="https://linkedin.com/in/mohit-jani-robotics" target="_blank" class="btn-outline">🔗 LinkedIn</a>
      <a href="https://github.com/mohitjani" target="_blank" class="btn-outline">🐙 GitHub</a>
      <a href="mailto:mohit10.jani@gmail.com" class="btn-outline">📧 Email Me</a>
    </div>
    <p style="margin-top: 1.5rem;">📍 Based in Surat, India | Open to BCI & advanced robotics collaborations</p>
  </div>

  <footer>
    <p>Mohit Jani — Design & Development Engineer (Robotics, Vision, Precision Assembly) © 2026</p>
  </footer>
</div>

<script>
  // Smooth scroll to sections when clicking nav buttons
  document.querySelectorAll('.nav-btn').forEach(btn => {
    btn.addEventListener('click', (e) => {
      const sectionId = btn.getAttribute('data-section');
      let targetElement = null;
      if (sectionId === 'about') targetElement = document.getElementById('about');
      else if (sectionId === 'experience') targetElement = document.getElementById('experience-section');
      else if (sectionId === 'projects') targetElement = document.getElementById('projects-section');
      else if (sectionId === 'gallery') targetElement = document.getElementById('gallery-section');
      else if (sectionId === 'contact') targetElement = document.getElementById('contact-section');
      
      if (targetElement) {
        targetElement.scrollIntoView({ behavior: 'smooth', block: 'start' });
        // optional: add a small highlight effect
        targetElement.style.transition = 'background 0.3s';
        targetElement.style.background = '#f9fffae0';
        setTimeout(() => {
          targetElement.style.background = '';
        }, 600);
      } else {
        // fallback for about (hero)
        if (sectionId === 'about') {
          document.querySelector('.hero').scrollIntoView({ behavior: 'smooth' });
        }
      }
    });
  });

  // Additional dynamic: simple interactive console greeting
  console.log('Mohit Jani portfolio — Robotics engineer | images, videos & smooth navigation active');
</script>

<!-- 
  Notes: 
  - Images are placeholder.cc placeholders with descriptive text but can be replaced by real images in production.
  - Video samples use external sample videos (common Google bucket) for demonstration — Mohit can replace with actual project recordings.
  - All gallery items show images/videos for each project. Added two extra image rows to highlight work.
  - Buttons on top navigate to about, experience, projects, media gallery, contact.
  - fully responsive, with hover effects.
-->
</body>
</html>
