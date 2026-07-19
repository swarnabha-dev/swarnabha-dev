<div align="center">

```aura width=860 height=200
 <div style={{ width: '100%', height: '100%', background: '#08080c', display: 'flex', alignItems: 'center', fontFamily: 'Inter', position: 'relative', overflow: 'hidden', borderRadius: 16, border: '1px solid rgba(110,80,220,0.18)' }}>
 <style>
   {`
     @keyframes float-slow { 0%, 100% { transform: translateX(0px); opacity: 0.8; } 50% { transform: translateX(350px); opacity: 1.2; } }
     @keyframes float-medium { 0%, 100% { transform: translateX(0px); opacity: 0.7; } 50% { transform: translateX(-250px); opacity: 1.1; } }
     @keyframes float-fast { 0%, 100% { transform: translateX(0px); opacity: 0.9; } 50% { transform: translateX(200px); opacity: 0.6; } }
     @keyframes float-pulse { 0%, 100% { transform: scale(1); opacity: 0.8; } 50% { transform: scale(1.3); opacity: 0.4; } }
     #glow-1 { animation: float-slow 8s ease-in-out infinite; }
     #glow-2 { animation: float-medium 12s ease-in-out infinite; }
     #glow-3 { animation: float-fast 9s ease-in-out infinite; }
     #glow-4 { animation: float-slow 11s ease-in-out infinite reverse; }
     #glow-8 { animation: float-pulse 7s ease-in-out infinite; }
   `}
 </style>
 <svg width="860" height="200" style={{ position: 'absolute', top: 0, left: 0 }}>
   <defs>
     <radialGradient id="g1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(110,20,210,0.72)" /><stop offset="70%" stopColor="rgba(90,15,180,0)" /></radialGradient>
     <radialGradient id="g2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(40,60,255,0.6)" /><stop offset="70%" stopColor="rgba(30,50,200,0)" /></radialGradient>
     <radialGradient id="g3" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(0,130,255,0.45)" /><stop offset="70%" stopColor="rgba(0,100,220,0)" /></radialGradient>
   </defs>
   <ellipse id="glow-1" cx="180" cy="230" rx="260" ry="190" fill="url(#g1)" />
   <ellipse id="glow-2" cx="300" cy="240" rx="220" ry="160" fill="url(#g2)" />
   <ellipse id="glow-3" cx="420" cy="240" rx="180" ry="140" fill="url(#g3)" />
   <ellipse id="glow-8" cx="590" cy="250" rx="150" ry="130" fill="url(#g1)" />
 </svg>
 <div style={{ position: 'absolute', left: 48, top: 52, width: 96, height: 96, borderRadius: 48, background: 'linear-gradient(135deg, #6622ee, #0088ff)', display: 'flex', alignItems: 'center', justifyContent: 'center' }}>
   <img src={(github && github.user && github.user.avatarUrl) || 'https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png'} width={88} height={88} style={{ borderRadius: 44 }} />
 </div>
 <div style={{ display:'flex', flexDirection:'column', marginLeft:168, gap:8 }}>
   <div style={{ display:'flex', fontSize:38, fontWeight:800, color:'#ffffff', letterSpacing:'-1px', lineHeight:1 }}>
     {(github && github.user && (github.user.name || github.user.login)) || 'Swarnabha Halder'}
   </div>
   <div style={{ display:'flex', fontSize:15, color:'rgba(180,165,255,0.8)', fontWeight:400, letterSpacing:'0.3px' }}>
     AI Engineer · Backend Developer · Researcher
   </div>
   <div style={{ display:'flex', gap:8, marginTop:6 }}>
     {['Python', 'FastAPI', 'PyTorch', 'C++'].map(function(tag) {
       return (
         <div key={tag} style={{ display:'flex', padding:'4px 12px', borderRadius:20, background:'rgba(80,40,220,0.18)', border:'1px solid rgba(100,70,240,0.32)', color:'rgba(205,195,255,0.85)', fontSize:12, fontWeight:600 }}>{tag}</div>
       );
     })}
   </div>
 </div>
</div>
```

<br>

```aura width=100 height=44 link="https://github.com/swarnabha-dev" inline align=center
<SocialMediaButton icon="https://cdn.simpleicons.org/github/ffffff" text="GitHub" backgroundColor="#141414" textColor="#ffffff" width={100} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#141414' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#ffffff' }, { offset: '65%', color: '#141414' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
```aura width=100 height=44 link="https://x.com/swarnabha_dev" inline
<SocialMediaButton icon="https://cdn.simpleicons.org/x/ffffff" text="X" backgroundColor="#141414" textColor="#ffffff" width={100} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#141414' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#ffffff' }, { offset: '65%', color: '#141414' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
```aura width=120 height=44 link="https://linkedin.com/in/swarnabha-halder-627692254" inline
<SocialMediaButton icon="https://cdn.simpleicons.org/linkedin/0A66C2" text="LinkedIn" backgroundColor="#041221" textColor="#ffffff" width={120} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#041221' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#0A66C2' }, { offset: '65%', color: '#041221' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={20} />
```
```aura width=110 height=44 link="mailto:swarnabha@swarnabha.tech" inline
<SocialMediaButton icon="https://cdn.simpleicons.org/gmail/EA4335" text="Email" backgroundColor="#330e0b" textColor="#ffffff" width={110} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#330e0b' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#EA4335' }, { offset: '65%', color: '#330e0b' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={20} />
```

<br>

<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira%20Code&weight=600&size=20&duration=4000&pause=1000&color=7AA2F7&center=true&vCenter=true&width=600&lines=Medical%20Image%20Registration;Secure%20FastAPI%20Analytics;Planetary%20Material%20Prediction;Financial%20Market%20Modeling;Production-grade%20AI%20Systems" alt="Typing SVG" />
</a>

<br>

```aura width=860 height=420
(function() {
  return (
    <div style={{ width: '100%', height: '100%', display: 'flex', alignItems: 'center', justifyContent: 'center', position: 'relative' }}>
      <style>
        {`
          @keyframes float-char { 0%, 100% { transform: translateY(0px); } 50% { transform: translateY(-25px); } }
          @keyframes pulse-aura { 0%, 100% { opacity: 0.3; transform: scale(1); } 50% { opacity: 0.7; transform: scale(1.15); } }
          #char-group { animation: float-char 6s ease-in-out infinite; }
          #aura-glow { animation: pulse-aura 5s ease-in-out infinite; }
        `}
      </style>
      <svg width="860" height="420" style={{ position: 'absolute', top: 0, left: 0 }}>
        <defs>
          <radialGradient id="char-bg" cx="50%" cy="50%" r="50%">
            <stop offset="0%" stopColor="rgba(120,40,240,0.6)" />
            <stop offset="40%" stopColor="rgba(90,20,180,0.2)" />
            <stop offset="70%" stopColor="transparent" />
          </radialGradient>
          <clipPath id="circle-clip">
            <circle cx="430" cy="210" r="160" />
          </clipPath>
        </defs>
        <ellipse id="aura-glow" cx="430" cy="210" rx="220" ry="220" fill="url(#char-bg)" />
        <g id="char-group">
          <image href="https://github.com/user-attachments/assets/af00b81f-0143-42ab-9010-e2fa8ef0e424" width="320" height="320" x="270" y="50" preserveAspectRatio="xMidYMid slice" clipPath="url(#circle-clip)" />
          <circle cx="430" cy="210" r="160" fill="none" stroke="rgba(180,140,255,0.7)" strokeWidth="4" />
        </g>
      </svg>
    </div>
  );
})()
```

</div>

---

```aura width=860 height=80
<div style={{ width: '100%', height: '100%', background: '#08080c', display: 'flex', alignItems: 'center', justifyContent: 'center', position: 'relative', overflow: 'hidden', borderRadius: 12, border: '1px solid rgba(110,80,220,0.2)' }}>
  <style>{` @keyframes pulse-text { 0%, 100% { text-shadow: 0 0 10px rgba(110,80,220,0.5); } 50% { text-shadow: 0 0 25px rgba(160,100,255,0.9); } } #title { animation: pulse-text 3s infinite; } `}</style>
  <svg width="860" height="80" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs><radialGradient id="bg" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(110,40,240,0.3)" /><stop offset="100%" stopColor="transparent" /></radialGradient></defs>
    <rect width="860" height="80" fill="url(#bg)" />
  </svg>
  <h2 id="title" style={{ color: '#fff', fontFamily: 'Inter', fontSize: 26, fontWeight: 700, letterSpacing: '3px', margin: 0, display: 'flex' }}>ABOUT ME</h2>
</div>
```

My work spans **scientific computing, distributed backend systems, medical image analysis, and modern AI infrastructure**. I enjoy turning complex research prototypes into reliable, secure, and maintainable products. 

- 🎓 **Education:** M.Tech in Computer Science, Indian Statistical Institute (ISI) | B.Tech in CSE
- 🎯 **Current Focus:** Building highly available, asynchronous API architectures and enterprise-grade AI deployments.
- 🌱 **Currently Exploring:** Agentic AI, Multi-Agent Systems, RAG Pipelines, and Vector Databases.
- 💼 **Open To:** Roles in AI Engineering, Backend Architecture, and Applied Research.

---

```aura width=860 height=80
<div style={{ width: '100%', height: '100%', background: '#08080c', display: 'flex', alignItems: 'center', justifyContent: 'center', position: 'relative', overflow: 'hidden', borderRadius: 12, border: '1px solid rgba(110,80,220,0.2)' }}>
  <style>{` @keyframes pulse-text2 { 0%, 100% { text-shadow: 0 0 10px rgba(40,110,240,0.5); } 50% { text-shadow: 0 0 25px rgba(80,160,255,0.9); } } #title2 { animation: pulse-text2 3s infinite; } `}</style>
  <svg width="860" height="80" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs><radialGradient id="bg2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(40,110,240,0.25)" /><stop offset="100%" stopColor="transparent" /></radialGradient></defs>
    <rect width="860" height="80" fill="url(#bg2)" />
  </svg>
  <h2 id="title2" style={{ color: '#fff', fontFamily: 'Inter', fontSize: 26, fontWeight: 700, letterSpacing: '3px', margin: 0, display: 'flex' }}>FEATURED PROJECTS</h2>
</div>
```

### 🔐 PrintFlow: Secure Print Analytics and Management Platform
**Enterprise-grade analytics system with robust security architectures.**
* **Stack:** FastAPI, MySQL, Windows Event Logs
* **Highlights:** Implemented mTLS authentication and secure JWT authorization pipelines. Designed a high-performance asynchronous backend capable of scaling enterprise print telemetry data.

### 🏥 Medical Image Registration
**Advanced algorithmic pipeline for precision medical imaging.**
* **Stack:** OpenCV, Python, Scientific Computing Libraries
* **Highlights:** Engineered B-Spline and Demons registration models. Applied research to 3D reconstruction and histopathology to improve automated diagnostic accuracy.

### 🌍 CosmoCompute: Planetary Material Predictor
**Predictive modeling system for planetary materials.**
* **Stack:** PyTorch, Interactive Dashboards, Data Engineering
* **Highlights:** Processed and analyzed massive NASA datasets to build robust machine learning models for geological material prediction. 

### 👁️ AuthVision
**AI-powered attendance and spoof-detection system.**
* **Stack:** TensorFlow, YOLO, FastAPI, Docker, JWT
* **Highlights:** Designed an end-to-end computer vision pipeline with integrated anti-spoofing mechanisms, containerized for rapid, scalable production deployment.

---

```aura width=860 height=80
<div style={{ width: '100%', height: '100%', background: '#08080c', display: 'flex', alignItems: 'center', justifyContent: 'center', position: 'relative', overflow: 'hidden', borderRadius: 12, border: '1px solid rgba(110,80,220,0.2)' }}>
  <style>{` @keyframes pulse-text3 { 0%, 100% { text-shadow: 0 0 10px rgba(240,40,140,0.5); } 50% { text-shadow: 0 0 25px rgba(255,80,180,0.9); } } #title3 { animation: pulse-text3 3s infinite; } `}</style>
  <svg width="860" height="80" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs><radialGradient id="bg3" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(240,40,140,0.25)" /><stop offset="100%" stopColor="transparent" /></radialGradient></defs>
    <rect width="860" height="80" fill="url(#bg3)" />
  </svg>
  <h2 id="title3" style={{ color: '#fff', fontFamily: 'Inter', fontSize: 26, fontWeight: 700, letterSpacing: '3px', margin: 0, display: 'flex' }}>TECHNICAL ARSENAL</h2>
</div>
```

<div align="center">
<br>

```aura width=100 height=44 inline align=center
<SocialMediaButton icon="https://cdn.simpleicons.org/python/3776AB" text="Python" backgroundColor="#0e1e2b" textColor="#ffffff" width={100} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#0e1e2b' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#3776AB' }, { offset: '65%', color: '#0e1e2b' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
```aura width=100 height=44 inline
<SocialMediaButton icon="https://cdn.simpleicons.org/c/A8B9CC" text="C" backgroundColor="#2a2e33" textColor="#ffffff" width={100} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#2a2e33' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#A8B9CC' }, { offset: '65%', color: '#2a2e33' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
```aura width=100 height=44 inline
<SocialMediaButton icon="https://cdn.simpleicons.org/cplusplus/00599C" text="C++" backgroundColor="#001627" textColor="#ffffff" width={100} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#001627' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#00599C' }, { offset: '65%', color: '#001627' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
```aura width=100 height=44 inline
<SocialMediaButton icon="https://cdn.simpleicons.org/fastapi/009688" text="FastAPI" backgroundColor="#001e1b" textColor="#ffffff" width={100} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#001e1b' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#009688' }, { offset: '65%', color: '#001e1b' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```

<br>

```aura width=100 height=44 inline align=center
<SocialMediaButton icon="https://cdn.simpleicons.org/django/092E20" text="Django" backgroundColor="#020c08" textColor="#ffffff" width={100} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#020c08' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#092E20' }, { offset: '65%', color: '#020c08' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
```aura width=100 height=44 inline
<SocialMediaButton icon="https://cdn.simpleicons.org/flask/3BABC3" text="Flask" backgroundColor="#0f2b31" textColor="#ffffff" width={100} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#0f2b31' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#3BABC3' }, { offset: '65%', color: '#0f2b31' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
```aura width=110 height=44 inline
<SocialMediaButton icon="https://cdn.simpleicons.org/mongodb/47A248" text="MongoDB" backgroundColor="#122912" textColor="#ffffff" width={110} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#122912' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#47A248' }, { offset: '65%', color: '#122912' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
```aura width=100 height=44 inline
<SocialMediaButton icon="https://cdn.simpleicons.org/mysql/4479A1" text="MySQL" backgroundColor="#111e28" textColor="#ffffff" width={100} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#111e28' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#4479A1' }, { offset: '65%', color: '#111e28' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```

<br>

```aura width=140 height=44 inline align=center
<SocialMediaButton icon="https://cdn.simpleicons.org/cloudflare/F38020" text="Cloudflare" backgroundColor="#3d2008" textColor="#ffffff" width={140} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#3d2008' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#F38020' }, { offset: '65%', color: '#3d2008' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
```aura width=100 height=44 inline
<SocialMediaButton icon="https://cdn.simpleicons.org/docker/2496ED" text="Docker" backgroundColor="#071e2f" textColor="#ffffff" width={100} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#071e2f' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#2496ED' }, { offset: '65%', color: '#071e2f' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
```aura width=100 height=44 inline
<SocialMediaButton icon="https://cdn.simpleicons.org/ubuntu/E95420" text="Ubuntu" backgroundColor="#3a1508" textColor="#ffffff" width={100} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#3a1508' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#E95420' }, { offset: '65%', color: '#3a1508' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
</div>

---

```aura width=860 height=80
<div style={{ width: '100%', height: '100%', background: '#08080c', display: 'flex', alignItems: 'center', justifyContent: 'center', position: 'relative', overflow: 'hidden', borderRadius: 12, border: '1px solid rgba(110,80,220,0.2)' }}>
  <style>{` @keyframes pulse-text4 { 0%, 100% { text-shadow: 0 0 10px rgba(110,240,140,0.5); } 50% { text-shadow: 0 0 25px rgba(80,255,180,0.9); } } #title4 { animation: pulse-text4 3s infinite; } `}</style>
  <svg width="860" height="80" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs><radialGradient id="bg4" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(110,240,140,0.25)" /><stop offset="100%" stopColor="transparent" /></radialGradient></defs>
    <rect width="860" height="80" fill="url(#bg4)" />
  </svg>
  <h2 id="title4" style={{ color: '#fff', fontFamily: 'Inter', fontSize: 26, fontWeight: 700, letterSpacing: '3px', margin: 0, display: 'flex' }}>EXPERIENCE & JOURNEY</h2>
</div>
```

- **2026** — M.Tech CS at Indian Statistical Institute (ISI) 
- **2025** — Research Internship at Indian Statistical Institute (ISI) | Planetary Material Prediction | Medical Image Registration Research
- **2024** — Backend Engineering at TechnoHacks & CodeSoft
- **2023** — Active Open Source Contributions (Hacktoberfest '23 & '24)
- **2022** — Began Open Source Journey & Competitive Programming

---

```aura width=860 height=80
<div style={{ width: '100%', height: '100%', background: '#08080c', display: 'flex', alignItems: 'center', justifyContent: 'center', position: 'relative', overflow: 'hidden', borderRadius: 12, border: '1px solid rgba(110,80,220,0.2)' }}>
  <style>{` @keyframes pulse-text5 { 0%, 100% { text-shadow: 0 0 10px rgba(240,180,40,0.5); } 50% { text-shadow: 0 0 25px rgba(255,200,80,0.9); } } #title5 { animation: pulse-text5 3s infinite; } `}</style>
  <svg width="860" height="80" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs><radialGradient id="bg5" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(240,180,40,0.25)" /><stop offset="100%" stopColor="transparent" /></radialGradient></defs>
    <rect width="860" height="80" fill="url(#bg5)" />
  </svg>
  <h2 id="title5" style={{ color: '#fff', fontFamily: 'Inter', fontSize: 26, fontWeight: 700, letterSpacing: '3px', margin: 0, display: 'flex' }}>GITHUB ANALYTICS</h2>
</div>
```

<div align="center">

<br>

<a href="https://github.com/stats-organization/github-stats-extended">
  <img src="https://github-stats-extended.vercel.app/api?username=swarnabha-dev&theme=tokyonight" alt="Swarnabha's GitHub stats" height="180" />
</a>
<br>
<img src="https://streak-stats.demolab.com/?user=swarnabha-dev&theme=tokyonight&hide_border=true&title_color=7AA2F7&ring=7AA2F7&fire=7AA2F7" height="180" alt="GitHub Streak" />
<br>
<a href="https://github.com/ashutosh00710/github-readme-activity-graph">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=swarnabha-dev&theme=tokyo-night&hide_border=true&color=7AA2F7" width="80%" alt="Activity Graph" />
</a>
<br><br>

## 🤝 Let's Connect
**[Explore My Portfolio](https://swarnabha.tech/) • [Connect on LinkedIn](https://linkedin.com/in/swarnabha-halder-627692254)**

<br>
<a href="https://github.com/piyushsuthar/github-readme-quotes">
  <img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=tokyonight" alt="Dynamic Programming Quote" />
</a>

<p align="center"><sub>𝗉𝗈𝗐𝖾𝗋𝖾𝖽 𝖻𝗒 <a href="https://github.com/collectioneur/readme-aura">𝗋𝖾𝖺𝖽𝗆𝖾-𝖺𝗎𝗋𝖺</a></sub></p>
</div>
