```markdown
<div align="center">

```aura width=800 height=300
<div style={{ display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', height: '100%', fontFamily: 'sans-serif', color: '#f5f5f5', backgroundColor: '#11111b' }}>
  <style>
    {`
      @keyframes float {
        0%, 100% { transform: translateY(0px); }
        50% { transform: translateY(-10px); }
      }
      @keyframes gradientPulse {
        0% { stop-color: #7AA2F7; }
        50% { stop-color: #BB9AF7; }
        100% { stop-color: #7AA2F7; }
      }
      #hero-badge { animation: float 6s ease-in-out infinite; }
      #glow-stop-1 { animation: gradientPulse 4s ease-in-out infinite; }
    `}
  </style>
  <svg width="0" height="0">
    <defs>
      <linearGradient id="heroGradient" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop id="glow-stop-1" offset="0%" stop-color="#7AA2F7" />
        <stop offset="100%" stop-color="#11111b" />
      </linearGradient>
    </defs>
  </svg>

  <div id="hero-badge" style={{ display: 'flex', padding: '10px 20px', borderRadius: '50px', border: '1px solid #7AA2F7', backgroundColor: 'rgba(122, 162, 247, 0.1)', marginBottom: '20px', fontSize: '14px', fontWeight: '600', letterSpacing: '1px' }}>
    AVAILABLE FOR COLLABORATION
  </div>

  <h1 style={{ fontSize: '48px', margin: '0 0 10px 0', fontWeight: '800' }}>
    Swarnabha <span style={{ color: '#7AA2F7' }}>Halder</span>
  </h1>
  <h2 style={{ fontSize: '24px', margin: '0 0 20px 0', fontWeight: '400', color: '#a9b1d6' }}>
    AI Engineer • Backend Developer • Researcher
  </h2>
  
  <p style={{ fontSize: '16px', color: '#9aa5ce', maxWidth: '600px', textAlign: 'center', lineHeight: '1.5', margin: '0' }}>
    I build production-grade AI systems where mathematics meets scalable software engineering.
  </p>
</div>

```





---

##  About Me

My work spans **scientific computing, distributed backend systems, medical image analysis, and modern AI infrastructure**. I enjoy turning complex research prototypes into reliable, secure, and maintainable products.

* 🎓 **Education:** M.Tech in Computer Science, Indian Statistical Institute (ISI) | B.Tech in CSE
* 🎯 **Current Focus:** Building highly available, asynchronous API architectures and enterprise-grade AI deployments.
* 🌱 **Currently Exploring:** Agentic AI, Multi-Agent Systems, RAG Pipelines, and Vector Databases.
* 💼 **Open To:** Roles in AI Engineering, Backend Architecture, and Applied Research.

---

##  Featured Engineering Projects

```aura width=800 height=450
<div style={{ display: 'flex', flexWrap: 'wrap', gap: '20px', padding: '20px', fontFamily: 'sans-serif', backgroundColor: '#11111b' }}>
  
  <style>
    {`
      @keyframes slideUp {
        from { transform: translateY(20px); opacity: 0; }
        to { transform: translateY(0); opacity: 1; }
      }
      .project-card {
        display: flex;
        flex-direction: column;
        width: calc(50% - 10px);
        background-color: #1e1e2e;
        border-radius: 12px;
        padding: 20px;
        border: 1px solid #313244;
        box-sizing: border-box;
      }
      #card-1 { animation: slideUp 0.6s ease-out forwards; }
      #card-2 { animation: slideUp 0.6s ease-out 0.2s forwards; opacity: 0; }
      #card-3 { animation: slideUp 0.6s ease-out 0.4s forwards; opacity: 0; }
      #card-4 { animation: slideUp 0.6s ease-out 0.6s forwards; opacity: 0; }
    `}
  </style>

  {/* Card 1 */}
  <div id="card-1" className="project-card">
    <div style={{ display: 'flex', alignItems: 'center', marginBottom: '10px' }}>
      <div style={{ fontSize: '24px', marginRight: '10px' }}>🔐</div>
      <h3 style={{ margin: 0, color: '#f5f5f5', fontSize: '18px' }}>Secure Print Analytics</h3>
    </div>
    <p style={{ color: '#a9b1d6', fontSize: '14px', lineHeight: '1.4', margin: '0 0 15px 0', flexGrow: 1 }}>
      Enterprise API architecture implementing mTLS and secure JWT pipelines for scalable telemetry.
    </p>
    <div style={{ display: 'flex', gap: '8px' }}>
      <span style={{ padding: '4px 8px', borderRadius: '4px', backgroundColor: '#313244', color: '#7AA2F7', fontSize: '12px' }}>FastAPI</span>
      <span style={{ padding: '4px 8px', borderRadius: '4px', backgroundColor: '#313244', color: '#7AA2F7', fontSize: '12px' }}>MySQL</span>
    </div>
  </div>

  {/* Card 2 */}
  <div id="card-2" className="project-card">
    <div style={{ display: 'flex', alignItems: 'center', marginBottom: '10px' }}>
      <div style={{ fontSize: '24px', marginRight: '10px' }}>🏥</div>
      <h3 style={{ margin: 0, color: '#f5f5f5', fontSize: '18px' }}>Medical Registration</h3>
    </div>
    <p style={{ color: '#a9b1d6', fontSize: '14px', lineHeight: '1.4', margin: '0 0 15px 0', flexGrow: 1 }}>
      Engineered B-Spline models and 3D reconstruction pipelines to improve diagnostic accuracy.
    </p>
    <div style={{ display: 'flex', gap: '8px' }}>
      <span style={{ padding: '4px 8px', borderRadius: '4px', backgroundColor: '#313244', color: '#BB9AF7', fontSize: '12px' }}>OpenCV</span>
      <span style={{ padding: '4px 8px', borderRadius: '4px', backgroundColor: '#313244', color: '#BB9AF7', fontSize: '12px' }}>Python</span>
    </div>
  </div>

  {/* Card 3 */}
  <div id="card-3" className="project-card">
    <div style={{ display: 'flex', alignItems: 'center', marginBottom: '10px' }}>
      <div style={{ fontSize: '24px', marginRight: '10px' }}>🌍</div>
      <h3 style={{ margin: 0, color: '#f5f5f5', fontSize: '18px' }}>CosmoCompute</h3>
    </div>
    <p style={{ color: '#a9b1d6', fontSize: '14px', lineHeight: '1.4', margin: '0 0 15px 0', flexGrow: 1 }}>
      Processed massive NASA datasets to build robust ML models for planetary material prediction.
    </p>
    <div style={{ display: 'flex', gap: '8px' }}>
      <span style={{ padding: '4px 8px', borderRadius: '4px', backgroundColor: '#313244', color: '#7DCFFF', fontSize: '12px' }}>PyTorch</span>
      <span style={{ padding: '4px 8px', borderRadius: '4px', backgroundColor: '#313244', color: '#7DCFFF', fontSize: '12px' }}>Data Eng</span>
    </div>
  </div>

  {/* Card 4 */}
  <div id="card-4" className="project-card">
    <div style={{ display: 'flex', alignItems: 'center', marginBottom: '10px' }}>
      <div style={{ fontSize: '24px', marginRight: '10px' }}>👁️</div>
      <h3 style={{ margin: 0, color: '#f5f5f5', fontSize: '18px' }}>AuthVision</h3>
    </div>
    <p style={{ color: '#a9b1d6', fontSize: '14px', lineHeight: '1.4', margin: '0 0 15px 0', flexGrow: 1 }}>
      End-to-end CV pipeline with anti-spoofing mechanisms, containerized for rapid deployment.
    </p>
    <div style={{ display: 'flex', gap: '8px' }}>
      <span style={{ padding: '4px 8px', borderRadius: '4px', backgroundColor: '#313244', color: '#F7768E', fontSize: '12px' }}>TensorFlow</span>
      <span style={{ padding: '4px 8px', borderRadius: '4px', backgroundColor: '#313244', color: '#F7768E', fontSize: '12px' }}>YOLO</span>
    </div>
  </div>

</div>

```

---

##  Technical Arsenal

### Languages

### Backend & Frameworks

### AI & Machine Learning

### Cloud, Infra & Databases

### Tooling

---

## ⏳ Experience & Journey

* **2025** — M.Tech CS at Indian Statistical Institute (ISI) | Medical Image Registration Research
* **2024** — Backend Engineering at TechnoHacks & CodeSoft
* **2023** — Active Open Source Contributions (Hacktoberfest '23 & '24)
* **2022** — Began Open Source Journey & Competitive Programming

---

##  GitHub Analytics









---

##  Let's Connect

**[Explore My Portfolio](https://swarnabha.tech/) • [Connect on LinkedIn**](https://linkedin.com/in/swarnabha-halder-627692254)





> *"Good engineering isn't about writing more code—it's about designing systems that remain reliable, scalable, and understandable long after they're deployed."*
