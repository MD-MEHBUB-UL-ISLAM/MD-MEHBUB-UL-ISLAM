<div align="center">

<!-- Animated Background & Header -->
<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body {
    background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
    background-size: 400% 400%;
    animation: gradient 15s ease infinite;
    min-height: 100vh;
  }

  @keyframes gradient {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  .animated-text {
    background: linear-gradient(45deg, #DD0031, #FF6B9D, #FFC837, #FF6B9D, #DD0031);
    background-size: 300% 300%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    animation: shimmer 3s ease-in-out infinite;
    font-weight: 700;
    font-size: 3em;
  }

  @keyframes shimmer {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
  }

  .typing-effect {
    border-right: 3px solid #DD0031;
    animation: typing 3.5s steps(40, end), blink-caret 0.75s step-end infinite;
    white-space: nowrap;
    overflow: hidden;
  }

  @keyframes typing {
    from { width: 0; }
    to { width: 100%; }
  }

  @keyframes blink-caret {
    from, to { border-color: transparent; }
    50% { border-color: #DD0031; }
  }

  .glass-card {
    background: rgba(255, 255, 255, 0.1);
    backdrop-filter: blur(10px);
    border: 1px solid rgba(255, 255, 255, 0.2);
    border-radius: 20px;
    padding: 30px;
    margin: 20px;
    box-shadow: 0 8px 32px rgba(31, 38, 135, 0.37);
    transition: all 0.3s ease;
    animation: slideUp 0.6s ease-out;
  }

  .glass-card:hover {
    transform: translateY(-10px);
    background: rgba(255, 255, 255, 0.15);
    box-shadow: 0 12px 40px rgba(31, 38, 135, 0.5);
  }

  @keyframes slideUp {
    from {
      opacity: 0;
      transform: translateY(30px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  .skill-badge {
    display: inline-block;
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    color: white;
    padding: 12px 24px;
    border-radius: 50px;
    margin: 8px;
    font-weight: 600;
    cursor: pointer;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(102, 126, 234, 0.4);
    position: relative;
    overflow: hidden;
  }

  .skill-badge::before {
    content: '';
    position: absolute;
    top: 0;
    left: -100%;
    width: 100%;
    height: 100%;
    background: rgba(255, 255, 255, 0.3);
    transition: left 0.5s;
  }

  .skill-badge:hover::before {
    left: 100%;
  }

  .skill-badge:hover {
    transform: translateY(-5px) scale(1.05);
    box-shadow: 0 6px 20px rgba(102, 126, 234, 0.6);
  }

  .package-card {
    background: rgba(255, 255, 255, 0.08);
    backdrop-filter: blur(10px);
    border: 1px solid rgba(255, 255, 255, 0.2);
    border-radius: 15px;
    padding: 25px;
    margin: 15px 0;
    transition: all 0.3s ease;
    animation: fadeInUp 0.6s ease-out;
    border-left: 4px solid transparent;
    background-image: linear-gradient(rgba(255, 255, 255, 0.08), rgba(255, 255, 255, 0.08)), 
                      linear-gradient(90deg, #DD0031, #FF6B9D);
    background-clip: padding-box, border-box;
    background-origin: padding-box, border-box;
  }

  @keyframes fadeInUp {
    from {
      opacity: 0;
      transform: translateY(20px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  .package-card:hover {
    transform: translateX(10px);
    background: rgba(255, 255, 255, 0.12);
    box-shadow: 0 8px 25px rgba(221, 0, 49, 0.3);
  }

  .stat-box {
    background: linear-gradient(135deg, rgba(221, 0, 49, 0.8), rgba(255, 107, 157, 0.8));
    padding: 20px 30px;
    border-radius: 15px;
    margin: 10px;
    display: inline-block;
    color: white;
    font-weight: 700;
    animation: popIn 0.6s cubic-bezier(0.68, -0.55, 0.265, 1.55);
  }

  @keyframes popIn {
    0% { transform: scale(0) rotate(-45deg); opacity: 0; }
    100% { transform: scale(1) rotate(0); opacity: 1; }
  }

  .pulse {
    animation: pulse 2s infinite;
  }

  @keyframes pulse {
    0%, 100% { opacity: 1; }
    50% { opacity: 0.7; }
  }

  .float {
    animation: float 3s ease-in-out infinite;
  }

  @keyframes float {
    0%, 100% { transform: translateY(0px); }
    50% { transform: translateY(-20px); }
  }

  .icon-bounce {
    animation: bounce 2s infinite;
  }

  @keyframes bounce {
    0%, 100% { transform: translateY(0); }
    50% { transform: translateY(-10px); }
  }

  .gradient-text {
    background: linear-gradient(90deg, #DD0031, #FF6B9D, #FFC837);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }

  .divider {
    height: 2px;
    background: linear-gradient(90deg, transparent, #DD0031, transparent);
    margin: 30px 0;
    animation: expand 0.8s ease-out;
  }

  @keyframes expand {
    from { width: 0; }
    to { width: 100%; }
  }

  .tech-stack-item {
    display: inline-block;
    margin: 10px;
    animation: fadeIn 0.6s ease-out;
  }

  @keyframes fadeIn {
    from { opacity: 0; }
    to { opacity: 1; }
  }

  .achievement-item {
    background: rgba(255, 255, 255, 0.05);
    border-left: 4px solid #DD0031;
    padding: 15px 20px;
    margin: 10px 0;
    border-radius: 8px;
    transition: all 0.3s ease;
    animation: slideInLeft 0.6s ease-out;
  }

  @keyframes slideInLeft {
    from {
      opacity: 0;
      transform: translateX(-30px);
    }
    to {
      opacity: 1;
      transform: translateX(0);
    }
  }

  .achievement-item:hover {
    background: rgba(255, 255, 255, 0.1);
    transform: translateX(10px);
    border-left-color: #FF6B9D;
  }

  h1, h2, h3 {
    color: white;
    text-shadow: 0 2px 10px rgba(0, 0, 0, 0.2);
  }

  p {
    color: rgba(255, 255, 255, 0.9);
  }

  a {
    color: #FFC837;
    text-decoration: none;
    transition: all 0.3s ease;
  }

  a:hover {
    color: #FF6B9D;
    text-decoration: underline;
  }

  .cta-button {
    background: linear-gradient(135deg, #DD0031, #FF6B9D);
    color: white;
    padding: 15px 40px;
    border: none;
    border-radius: 50px;
    font-size: 1.1em;
    font-weight: 700;
    cursor: pointer;
    transition: all 0.3s ease;
    box-shadow: 0 4px 15px rgba(221, 0, 49, 0.4);
    margin: 10px;
    animation: slideDown 0.6s ease-out;
  }

  @keyframes slideDown {
    from {
      opacity: 0;
      transform: translateY(-20px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }

  .cta-button:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 25px rgba(221, 0, 49, 0.6);
  }

  .stars {
    position: fixed;
    width: 2px;
    height: 2px;
    background: white;
    border-radius: 50%;
    animation: twinkle 3s infinite;
  }

  @keyframes twinkle {
    0%, 100% { opacity: 0.3; }
    50% { opacity: 1; }
  }
</style>

<!-- Header Section -->
<div style="margin: 40px 0;">
  <h1 class="animated-text">MD Mehbub Ul Islam</h1>
  <p style="font-size: 1.3em; margin: 20px 0;" class="typing-effect">Angular Developer • Open Source Creator • Performance Specialist</p>
</div>

<div class="divider"></div>

<!-- Stat Boxes -->
<div align="center" style="margin: 30px 0;">
  <div class="stat-box">📦 6+ Published Packages</div>
  <div class="stat-box">⚡ 100k+ Items @ 60 FPS</div>
  <div class="stat-box">🌍 Bilingual Applications</div>
  <div class="stat-box">🎯 Production-Ready Code</div>
</div>

<!-- CTA Buttons -->
<div align="center" style="margin: 30px 0;">
  <a href="https://linkedin.com/in/md-mehbub-ul-islam-17b852257" target="_blank">
    <button class="cta-button">💼 LinkedIn Profile</button>
  </a>
  <a href="https://github.com/MD-MEHBUB-UL-ISLAM" target="_blank">
    <button class="cta-button">🔗 GitHub Repository</button>
  </a>
  <a href="mailto:mdmehbubulislam@gmail.com">
    <button class="cta-button">✉️ Get in Touch</button>
  </a>
</div>

<div class="divider"></div>

<!-- About Me Section -->
<div class="glass-card" style="max-width: 900px; margin: 30px auto;">
  <h2 style="margin-bottom: 20px;">🎯 About Me</h2>
  <p style="font-size: 1.1em; line-height: 1.8;">
    I'm a <span class="gradient-text"><strong>frontend-focused Angular engineer</strong></span> with a passion for building high-performance, production-grade applications and reusable component libraries. My expertise spans modern Angular architecture (signals, standalone components), responsive UI design, internationalization, and performance optimization.
  </p>
</div>

<!-- Key Strengths -->
<div style="max-width: 900px; margin: 30px auto;">
  <h2 style="text-align: center; margin-bottom: 30px;">💪 Core Competencies</h2>
  <div class="glass-card">
    <div class="achievement-item">
      <h3>🏗️ Architecture & Design Patterns</h3>
      <p>Standalone components • Signal-based state management • Dependency injection optimization • Design system implementation</p>
    </div>
    <div class="achievement-item">
      <h3>⚡ Performance Optimization</h3>
      <p>Virtual scrolling (100k+ items @ 60 FPS) • Memory-efficient rendering • Bundle size optimization • Lazy loading strategies</p>
    </div>
    <div class="achievement-item">
      <h3>🌍 Scalability & i18n</h3>
      <p>Bilingual applications (EN/BN) • Responsive design systems • Reusable component libraries • Multi-tenant architecture</p>
    </div>
    <div class="achievement-item">
      <h3>🧪 Code Quality & Testing</h3>
      <p>TypeScript strict mode • RxJS reactive patterns • Maintainable, production-ready code • Best practice implementation</p>
    </div>
  </div>
</div>

<div class="divider"></div>

<!-- Featured Packages -->
<div style="max-width: 1000px; margin: 30px auto;">
  <h2 style="text-align: center; margin-bottom: 30px;">📦 Featured npm Packages</h2>
  
  <div class="package-card">
    <h3>🚀 ngx-virtual-scroller</h3>
    <p>High-performance virtual scrolling for Angular. Render <strong>100k+ items at 60 FPS</strong> with constant memory usage.</p>
    <small><a href="https://github.com/MD-MEHBUB-UL-ISLAM/ngx-virtual-scroller" target="_blank">View Repository →</a></small>
  </div>

  <div class="package-card">
    <h3>🤖 ngx-ai-assist</h3>
    <p>AI-powered components featuring Chat, Autocomplete, Content Generator, and Sentiment Analysis with OpenAI streaming integration.</p>
    <small><a href="https://github.com/MD-MEHBUB-UL-ISLAM/ngx-ai-assist" target="_blank">View Repository →</a></small>
  </div>

  <div class="package-card">
    <h3>📋 ngx-dynamic-form-builder</h3>
    <p>JSON-driven dynamic form builder with validation, conditional logic, and 15+ customizable field types.</p>
    <small><a href="https://github.com/MD-MEHBUB-UL-ISLAM/ngx-dynamic-form-builder" target="_blank">View Repository →</a></small>
  </div>

  <div class="package-card">
    <h3>📅 ngx-date-range-picker</h3>
    <p>Bilingual (English/Bengali) date range picker with responsive design and seamless language toggle.</p>
    <small><a href="https://github.com/MD-MEHBUB-UL-ISLAM/ngx-date-range-picker" target="_blank">View Repository →</a></small>
  </div>

  <div class="package-card">
    <h3>🎥 ngx-video-recorder</h3>
    <p>Professional video/audio recording for Angular with pause/resume, playback controls, and device selection.</p>
    <small><a href="https://github.com/MD-MEHBUB-UL-ISLAM/ngx-video-recorder" target="_blank">View Repository →</a></small>
  </div>

  <div class="package-card">
    <h3>🛡️ ngx-attack-detector</h3>
    <p>Security monitoring component detecting script injection attacks in real-time.</p>
    <small><a href="https://github.com/MD-MEHBUB-UL-ISLAM/ngx-attack-detector" target="_blank">View Repository →</a></small>
  </div>
</div>

<div class="divider"></div>

<!-- Tech Stack -->
<div style="max-width: 900px; margin: 30px auto;">
  <h2 style="text-align: center; margin-bottom: 30px;">🛠️ Tech Stack</h2>
  <div class="glass-card" style="text-align: center;">
    <div style="margin: 20px 0;">
      <span class="skill-badge">Angular 19+</span>
      <span class="skill-badge">TypeScript</span>
      <span class="skill-badge">RxJS</span>
      <span class="skill-badge">Signals</span>
      <span class="skill-badge">Standalone Components</span>
    </div>
    <div style="margin: 20px 0;">
      <span class="skill-badge">Tailwind CSS</span>
      <span class="skill-badge">Responsive Design</span>
      <span class="skill-badge">HTML5/CSS3</span>
      <span class="skill-badge">JavaScript</span>
      <span class="skill-badge">Transloco i18n</span>
    </div>
    <div style="margin: 20px 0;">
      <span class="skill-badge">Node.js</span>
      <span class="skill-badge">Git</span>
      <span class="skill-badge">GitHub Actions</span>
      <span class="skill-badge">npm</span>
      <span class="skill-badge">Performance Optimization</span>
    </div>
  </div>
</div>

<div class="divider"></div>

<!-- Why Work With Me -->
<div style="max-width: 900px; margin: 30px auto;">
  <h2 style="text-align: center; margin-bottom: 30px;">✨ What You Get</h2>
  <div class="glass-card">
    <div class="achievement-item">
      ✅ <strong>Clean, maintainable code</strong> following SOLID principles and Angular best practices
    </div>
    <div class="achievement-item">
      ✅ <strong>Performance-first mindset</strong> with optimized rendering and bundle awareness
    </div>
    <div class="achievement-item">
      ✅ <strong>Reusable components</strong> that are well-documented and production-ready
    </div>
    <div class="achievement-item">
      ✅ <strong>Responsive expertise</strong> ensuring pixel-perfect designs across all devices
    </div>
    <div class="achievement-item">
      ✅ <strong>Bilingual support</strong> with seamless English/Bengali internationalization
    </div>
    <div class="achievement-item">
      ✅ <strong>Proactive problem solving</strong> identifying bottlenecks and implementing solutions
    </div>
  </div>
</div>

<div class="divider"></div>

<!-- Code Sample -->
<div style="max-width: 900px; margin: 30px auto;">
  <h2 style="text-align: center; margin-bottom: 30px;">💻 Modern Angular Patterns</h2>
  <div class="glass-card">
    <pre style="background: rgba(0,0,0,0.3); padding: 20px; border-radius: 10px; overflow-x: auto; color: #00FF00;">
<span style="color: #FF6B9D;">@Component</span>({
  selector: <span style="color: #FFC837;">'app-job-listing'</span>,
  standalone: <span style="color: #00FF00;">true</span>,
  template: <span style="color: #FFC837;">`
    @for (job of filteredJobs(); track job.id) {
      &lt;div class="job-card"&gt;
        {{ job.title }} - {{ formatSalary(job.salary) }}
      &lt;/div&gt;
    }
  `</span>
})
<span style="color: #FF6B9D;">export class</span> JobListingComponent {
  jobs = <span style="color: #FF6B9D;">signal</span>&lt;Job[]&gt;([]);
  searchTerm = <span style="color: #FF6B9D;">signal</span>(<span style="color: #FFC837;">''</span>);
  
  filteredJobs = <span style="color: #FF6B9D;">computed</span>(() =&gt;
    <span style="color: #FF6B9D;">this</span>.jobs().<span style="color: #00FF00;">filter</span>(j =&gt; 
      j.title.<span style="color: #00FF00;">includes</span>(<span style="color: #FF6B9D;">this</span>.searchTerm())
    )
  );
}</pre>
  </div>
</div>

<div class="divider"></div>

<!-- Achievements -->
<div style="max-width: 900px; margin: 30px auto;">
  <h2 style="text-align: center; margin-bottom: 30px;">🏆 Achievements</h2>
  <div class="glass-card">
    <div class="achievement-item">
      🎁 Published 6 npm packages solving real-world developer challenges
    </div>
    <div class="achievement-item">
      💡 Developed high-performance solutions rendering 100k+ items at 60 FPS
    </div>
    <div class="achievement-item">
      🌐 Built bilingual applications with seamless English/Bengali language switching
    </div>
    <div class="achievement-item">
      🚀 Optimized applications through virtual scrolling and reactive patterns
    </div>
    <div class="achievement-item">
      📚 Created reusable libraries with comprehensive documentation
    </div>
  </div>
</div>

<div class="divider"></div>

<!-- Call to Action -->
<div class="glass-card" style="max-width: 800px; margin: 50px auto; text-align: center;">
  <h2 class="gradient-text" style="-webkit-text-fill-color: transparent;">🚀 Let's Build Something Amazing</h2>
  <p style="font-size: 1.1em; margin: 20px 0;">Open to opportunities in Angular development, component libraries, and performance optimization roles.</p>
  
  <div style="margin: 30px 0;">
    <a href="https://linkedin.com/in/md-mehbub-ul-islam-17b852257" target="_blank">
      <button class="cta-button">Connect on LinkedIn</button>
    </a>
    <a href="mailto:mdmehbubulislam@gmail.com">
      <button class="cta-button">Send me an Email</button>
    </a>
  </div>

  <p style="font-style: italic; font-size: 0.95em; margin-top: 30px;">
    💻 "Code quality is not just about functionality—it's about creating maintainable solutions that scale with your team."
  </p>
</div>

<div style="height: 30px;"></div>

</div>

<!-- Footer Animation -->
<script>
// Create floating particles
const createParticles = () => {
  if (document.querySelectorAll('.stars').length > 20) return;
  
  for (let i = 0; i < 20; i++) {
    const star = document.createElement('div');
    star.className = 'stars';
    star.style.left = Math.random() * window.innerWidth + 'px';
    star.style.top = Math.random() * window.innerHeight + 'px';
    star.style.animationDelay = Math.random() * 3 + 's';
    document.body.appendChild(star);
  }
};

// Initialize on load
window.addEventListener('load', createParticles);
</script>
