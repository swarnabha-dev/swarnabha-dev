<div align="center">

```aura width=860 height=200
 <div style={{
 width: '100%', height: '100%', background: '#08080c',
 display: 'flex', alignItems: 'center', fontFamily: 'Inter',
 position: 'relative', overflow: 'hidden', borderRadius: 16,
 border: '1px solid rgba(110,80,220,0.18)'
}}>

 <style>
   {`
     @keyframes float-slow {
       0%, 100% { transform: translateX(0px); opacity: 0.8; }
       50% { transform: translateX(350px); opacity: 1.2; }
     }
     @keyframes float-medium {
       0%, 100% { transform: translateX(0px); opacity: 0.7; }
       50% { transform: translateX(-250px); opacity: 1.1; }
     }
     @keyframes float-fast {
       0%, 100% { transform: translateX(0px); opacity: 0.9; }
       50% { transform: translateX(200px); opacity: 0.6; }
     }
     @keyframes float-diagonal {
       0%, 100% { transform: translateX(0px); opacity: 0.75; }
       50% { transform: translateX(300px); opacity: 1.0; }
     }
     @keyframes float-wave {
       0%, 100% { transform: translateX(0px); opacity: 0.65; }
       33% { transform: translateX(-160px); opacity: 0.9; }
       66% { transform: translateX(80px); opacity: 1.0; }
     }
     @keyframes float-pulse {
       0%, 100% { transform: scale(1); opacity: 0.8; }
       50% { transform: scale(1.3); opacity: 0.4; }
     }
     #glow-1 { animation: float-slow 8s ease-in-out infinite; }
     #glow-2 { animation: float-medium 12s ease-in-out infinite; }
     #glow-3 { animation: float-fast 9s ease-in-out infinite; }
     #glow-4 { animation: float-slow 11s ease-in-out infinite reverse; }
     #glow-5 { animation: float-medium 14s ease-in-out infinite reverse; }
     #glow-6 { animation: float-diagonal 10s ease-in-out infinite; }
     #glow-7 { animation: float-wave 13s ease-in-out infinite; }
     #glow-8 { animation: float-pulse 7s ease-in-out infinite; }
   `}
 </style>

 <svg width="860" height="200" style={{ position: 'absolute', top: 0, left: 0 }}>
   <defs>
     <radialGradient id="g1" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(110,20,210,0.72)" />
       <stop offset="40%" stopColor="rgba(90,15,180,0.35)" />
       <stop offset="70%" stopColor="rgba(90,15,180,0)" />
     </radialGradient>
     <radialGradient id="g2" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(40,60,255,0.6)" />
       <stop offset="45%" stopColor="rgba(30,50,200,0.25)" />
       <stop offset="70%" stopColor="rgba(30,50,200,0)" />
     </radialGradient>
     <radialGradient id="g3" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(0,130,255,0.45)" />
       <stop offset="50%" stopColor="rgba(0,100,220,0.18)" />
       <stop offset="70%" stopColor="rgba(0,100,220,0)" />
     </radialGradient>
     <radialGradient id="g4" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(0,190,230,0.32)" />
       <stop offset="70%" stopColor="rgba(0,190,230,0)" />
     </radialGradient>
     <radialGradient id="g5" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(90,30,200,0.38)" />
       <stop offset="70%" stopColor="rgba(90,30,200,0)" />
     </radialGradient>
     <radialGradient id="g6" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(160,30,255,0.55)" />
       <stop offset="45%" stopColor="rgba(130,20,220,0.22)" />
       <stop offset="70%" stopColor="rgba(130,20,220,0)" />
     </radialGradient>
     <radialGradient id="g7" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(20,60,255,0.42)" />
       <stop offset="50%" stopColor="rgba(10,40,200,0.16)" />
       <stop offset="70%" stopColor="rgba(10,40,200,0)" />
     </radialGradient>
     <radialGradient id="g8" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(0,170,255,0.40)" />
       <stop offset="50%" stopColor="rgba(0,130,220,0.15)" />
       <stop offset="70%" stopColor="rgba(0,130,220,0)" />
     </radialGradient>
   </defs>

   <ellipse id="glow-1" cx="180" cy="230" rx="260" ry="190" fill="url(#g1)" />
   <ellipse id="glow-2" cx="300" cy="240" rx="220" ry="160" fill="url(#g2)" />
   <ellipse id="glow-3" cx="420" cy="240" rx="180" ry="140" fill="url(#g3)" />
   <ellipse id="glow-4" cx="550" cy="250" rx="150" ry="120" fill="url(#g4)" />
   <ellipse id="glow-5" cx="750" cy="250" rx="130" ry="110" fill="url(#g5)" />
   <ellipse id="glow-6" cx="300" cy="240" rx="180" ry="140" fill="url(#g6)" />
   <ellipse id="glow-7" cx="490" cy="230" rx="220" ry="170" fill="url(#g7)" />
   <ellipse id="glow-8" cx="590" cy="250" rx="150" ry="130" fill="url(#g8)" />
 </svg>

 <div style={{
   position: 'absolute', left: 48, top: 52, width: 96, height: 96,
   borderRadius: 48, background: 'linear-gradient(135deg, #6622ee, #0088ff)',
   display: 'flex', alignItems: 'center', justifyContent: 'center',
 }}>
   <img src={(github && github.user && github.user.avatarUrl) || 'https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png'} width={88} height={88} style={{ borderRadius: 44 }} />
 </div>

 <div style={{ display:'flex', flexDirection:'column', marginLeft:168, gap:8, zIndex: 10 }}>
   <div style={{ display:'flex', fontSize:38, fontWeight:800, color:'#ffffff', letterSpacing:'-1px', lineHeight:1 }}>
     {(github && github.user && (github.user.name || github.user.login)) || 'Swarnabha Halder'}
   </div>
   <div style={{ display:'flex', fontSize:15, color:'rgba(180,165,255,0.8)', fontWeight:400, letterSpacing:'0.3px' }}>
     AI Engineer · Backend Developer · Researcher
   </div>
   <div style={{ display:'flex', gap:8, marginTop:6 }}>
     {['Python', 'FastAPI', 'PyTorch', 'Docker', 'C++'].map(function(tag) {
       return (
         <div key={tag} style={{
           display:'flex', padding:'4px 12px', borderRadius:20,
           background:'rgba(80,40,220,0.18)', border:'1px solid rgba(100,70,240,0.32)',
           color:'rgba(205,195,255,0.85)', fontSize:12, fontWeight:600,
         }}>{tag}</div>
       );
     })}
   </div>
 </div>
</div>
```

<br>

```aura width=860 height=140
(function() {
 var stats = [
   { label: 'Repos', value: String((github && github.stats && github.stats.totalRepos) || 0), color: '#a78bfa' },
   { label: 'Stars', value: String((github && github.stats && github.stats.totalStars) || 0), color: '#60a5fa' },
   { label: 'Commits', value: String((github && github.stats && github.stats.totalCommits) || 0), color: '#f59e0b' },
 ];

 return (
   <div style={{
     width: '100%', height: '100%',
     background: '#08080c',
     display: 'flex', alignItems: 'center', justifyContent: 'center',
     fontFamily: 'Inter', borderRadius: 16,
     border: '1px solid rgba(110,80,220,0.18)',
     position: 'relative', overflow: 'hidden',
   }}>

     <style>
       {`
         @keyframes float-slow {
           0%, 100% { transform: translateX(0px); opacity: 0.8; }
           50% { transform: translateX(350px); opacity: 1.2; }
         }
         @keyframes float-medium {
           0%, 100% { transform: translateX(0px); opacity: 0.7; }
           50% { transform: translateX(-250px); opacity: 1.1; }
         }
         @keyframes float-fast {
           0%, 100% { transform: translateX(0px); opacity: 0.9; }
           50% { transform: translateX(200px); opacity: 0.6; }
         }
         @keyframes float-diagonal {
           0%, 100% { transform: translate(0px, 0px); opacity: 0.75; }
           50% { transform: translate(120px, 30px); opacity: 1.0; }
         }
         @keyframes float-wave {
           0%, 100% { transform: translateX(0px); opacity: 0.65; }
           33% { transform: translateX(-160px); opacity: 0.9; }
           66% { transform: translateX(80px); opacity: 1.0; }
         }
         @keyframes float-pulse {
           0%, 100% { transform: scale(1); opacity: 0.8; }
           50% { transform: scale(1.3); opacity: 0.4; }
         }
         #glow-1 { animation: float-slow 8s ease-in-out infinite; }
         #glow-2 { animation: float-medium 12s ease-in-out infinite; }
         #glow-3 { animation: float-fast 9s ease-in-out infinite; }
         #glow-4 { animation: float-diagonal 10s ease-in-out infinite; }
         #glow-5 { animation: float-wave 14s ease-in-out infinite; }
       `}
     </style>

     <svg width="860" height="140" style={{ position: 'absolute', top: 0, left: 0 }}>
       <defs>
         <radialGradient id="g1" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(110,20,210,0.65)" />
           <stop offset="45%" stopColor="rgba(80,15,170,0.28)" />
           <stop offset="70%" stopColor="rgba(80,15,170,0)" />
         </radialGradient>
         <radialGradient id="g2" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(40,70,255,0.55)" />
           <stop offset="45%" stopColor="rgba(20,50,200,0.22)" />
           <stop offset="70%" stopColor="rgba(20,50,200,0)" />
         </radialGradient>
         <radialGradient id="g3" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(0,140,255,0.42)" />
           <stop offset="70%" stopColor="rgba(0,140,255,0)" />
         </radialGradient>
         <radialGradient id="g4" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(0,195,235,0.30)" />
           <stop offset="70%" stopColor="rgba(0,195,235,0)" />
         </radialGradient>
         <radialGradient id="g5" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(100,30,210,0.40)" />
           <stop offset="70%" stopColor="rgba(100,30,210,0)" />
         </radialGradient>
       </defs>
       <ellipse id="glow-1" cx="710" cy="150" rx="210" ry="150" fill="url(#g1)" />
       <ellipse id="glow-2" cx="550" cy="140" rx="190" ry="140" fill="url(#g2)" />
       <ellipse id="glow-3" cx="400" cy="130" rx="170" ry="130" fill="url(#g3)" />
       <ellipse id="glow-4" cx="250" cy="140" rx="150" ry="120" fill="url(#g4)" />
       <ellipse id="glow-5" cx="100" cy="150" rx="130" ry="110" fill="url(#g5)" />
     </svg>

     {stats.map(function(s, i) {
       return (
         <div key={s.label} style={{
           flexGrow: 1, display: 'flex', flexDirection: 'column',
           alignItems: 'center', justifyContent: 'center',
           padding: '16px 8px',
           borderRight: i < stats.length - 1 ? '1px solid rgba(255,255,255,0.06)' : 'none',
           gap: 5,
         }}>
           <div style={{ display:'flex', fontSize:30, fontWeight:800, color:s.color, lineHeight:1 }}>
             {s.value}
           </div>
           <div style={{ display:'flex', fontSize:11, color:'rgba(200,195,225,0.45)', fontWeight:600, letterSpacing:'1.5px' }}>
             {s.label.toUpperCase()}
           </div>
         </div>
       );
     })}
   </div>
 );
})()
```
```aura width=100 height=44 link="https://github.com/swarnabha-dev" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/github/ffffff"
  text="GitHub"
  backgroundColor="#141414"
  textColor="#ffffff"
  width={100}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#141414' },
    { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#ffffff' },
    { offset: '65%', color: '#141414' }, { offset: '80%', color: '#888888' },
    { offset: '100%', color: '#444444' }
  ]}
  iconSize={22}
/>
```
```aura width=120 height=44 link="https://linkedin.com/in/swarnabha-halder-627692254" inline
<SocialMediaButton
  icon="https://cdn.simpleicons.org/linkedin/0A66C2"
  text="LinkedIn"
  backgroundColor="#041221"
  textColor="#ffffff"
  width={120}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#041221' },
    { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#0A66C2' },
    { offset: '65%', color: '#041221' }, { offset: '80%', color: '#888888' },
    { offset: '100%', color: '#444444' }
  ]}
  iconSize={20}
/>
```
```aura width=100 height=44 link="https://x.com/swarnabha_dev" inline
<SocialMediaButton
  icon="https://cdn.simpleicons.org/x/ffffff"
  text="X"
  backgroundColor="#141414"
  textColor="#ffffff"
  width={100}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#141414' },
    { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#ffffff' },
    { offset: '65%', color: '#141414' }, { offset: '80%', color: '#888888' },
    { offset: '100%', color: '#444444' }
  ]}
  iconSize={22}
/>
```

<br>

<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira%20Code&weight=600&size=20&duration=4000&pause=1000&color=7AA2F7&center=true&vCenter=true&width=600&lines=Medical%20Image%20Registration;Secure%20FastAPI%20Analytics;Planetary%20Material%20Prediction;Financial%20Market%20Modeling;Production-grade%20AI%20Systems" alt="Typing SVG" />
</a>

<br>

  <img alt="Swarnabha Character Illustration" src="https://github.com/user-attachments/assets/af00b81f-0143-42ab-9010-e2fa8ef0e424" width="450"  style="border-radius: 20px; box-shadow: 0px 10px 30px rgba(0,0,0,0.5);" />

</div>

---

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Travel%20and%20places/Rocket.png" alt="Rocket" width="30" height="30" /> About Me

My work spans **scientific computing, distributed backend systems, medical image analysis, and modern AI infrastructure**. I enjoy turning complex research prototypes into reliable, secure, and maintainable products. 

- 🎓 **Education:** M.Tech in Computer Science, Indian Statistical Institute (ISI) | B.Tech in CSE
- 🎯 **Current Focus:** Building highly available, asynchronous API architectures and enterprise-grade AI deployments.
- 🌱 **Currently Exploring:** Agentic AI, Multi-Agent Systems, RAG Pipelines, and Vector Databases.
- 💼 **Open To:** Roles in AI Engineering, Backend Architecture, and Applied Research.

---

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Activities/Sparkles.png" alt="Sparkles" width="30" height="30" /> Featured Engineering Projects

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

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Hammer%20and%20Wrench.png" alt="Hammer and Wrench" width="30" height="30" /> Technical Arsenal

<div align="center">

```aura width=860 height=168
(function() {
 var topLangs = (github && github.languages && github.languages.length > 0 ? github.languages.slice(0, 6).map(function(l) { return l.name; }) : ['Python', 'C++', 'Java', 'Bash', 'TypeScript', 'C']);
 var categories = [
   { title: 'Languages', color: '#a78bfa', items: topLangs },
   { title: 'Backend & AI', color: '#60a5fa', items: ['FastAPI', 'PyTorch', 'TensorFlow', 'OpenCV', 'Django'] },
 ];

 return (
   <div style={{
     width: '100%', height: '100%',
     background: '#08080c',
     display: 'flex', flexDirection: 'column',
     fontFamily: 'Inter', padding: '18px 32px', gap: 14,
     borderRadius: 16, border: '1px solid rgba(110,80,220,0.18)',
     position: 'relative', overflow: 'hidden',
   }}>

     <style>
       {`
         @keyframes float-slow {
           0%, 100% { transform: translateX(0px); opacity: 0.8; }
           50% { transform: translateX(350px); opacity: 1.2; }
         }
         @keyframes float-medium {
           0%, 100% { transform: translateX(0px); opacity: 0.7; }
           50% { transform: translateX(-250px); opacity: 1.1; }
         }
         @keyframes float-fast {
           0%, 100% { transform: translateX(0px); opacity: 0.9; }
           50% { transform: translateX(200px); opacity: 0.6; }
         }
         @keyframes float-diagonal {
           0%, 100% { transform: translate(0px, 0px); opacity: 0.75; }
           50% { transform: translate(120px, 30px); opacity: 1.0; }
         }
         @keyframes float-wave {
           0%, 100% { transform: translateX(0px); opacity: 0.65; }
           33% { transform: translateX(-160px); opacity: 0.9; }
           66% { transform: translateX(80px); opacity: 1.0; }
         }
         @keyframes float-pulse {
           0%, 100% { transform: scale(1); opacity: 0.8; }
           50% { transform: scale(1.3); opacity: 0.4; }
         }
         #glow-1 { animation: float-slow 9s ease-in-out infinite; }
         #glow-2 { animation: float-medium 12s ease-in-out infinite; }
         #glow-3 { animation: float-fast 8s ease-in-out infinite; }
         #glow-4 { animation: float-diagonal 11s ease-in-out infinite reverse; }
         #glow-5 { animation: float-wave 14s ease-in-out infinite reverse; }
         #glow-6 { animation: float-pulse 6s ease-in-out infinite; }
       `}
     </style>

     <svg width="860" height="168" style={{ position: 'absolute', top: 0, left: 0 }}>
       <defs>
         <radialGradient id="g1" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(115,20,215,0.68)" />
           <stop offset="42%" stopColor="rgba(85,15,175,0.30)" />
           <stop offset="70%" stopColor="rgba(85,15,175,0)" />
         </radialGradient>
         <radialGradient id="g2" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(55,55,255,0.55)" />
           <stop offset="45%" stopColor="rgba(35,45,210,0.22)" />
           <stop offset="70%" stopColor="rgba(35,45,210,0)" />
         </radialGradient>
         <radialGradient id="g3" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(0,130,255,0.42)" />
           <stop offset="50%" stopColor="rgba(0,100,220,0.16)" />
           <stop offset="70%" stopColor="rgba(0,100,220,0)" />
         </radialGradient>
         <radialGradient id="g4" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(0,185,240,0.32)" />
           <stop offset="70%" stopColor="rgba(0,185,240,0)" />
         </radialGradient>
         <radialGradient id="g5" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(100,25,205,0.42)" />
           <stop offset="70%" stopColor="rgba(100,25,205,0)" />
         </radialGradient>
         <radialGradient id="g6" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(60,80,255,0.35)" />
           <stop offset="70%" stopColor="rgba(60,80,255,0)" />
         </radialGradient>
       </defs>
       <ellipse id="glow-1" cx="170" cy="168" rx="260" ry="170" fill="url(#g1)" />
       <ellipse id="glow-2" cx="320" cy="178" rx="220" ry="140" fill="url(#g2)" />
       <ellipse id="glow-3" cx="460" cy="178" rx="190" ry="130" fill="url(#g3)" />
       <ellipse id="glow-4" cx="590" cy="188" rx="160" ry="110" fill="url(#g4)" />
       <ellipse id="glow-5" cx="750" cy="188" rx="140" ry="100" fill="url(#g5)" />
       <ellipse id="glow-6" cx="420" cy="138" rx="100" ry="80" fill="url(#g6)" />
     </svg>

     <div style={{ display:'flex', fontSize:10, fontWeight:700, color:'rgba(155,140,210,0.5)', letterSpacing:'3px' }}>
       TECH STACK
     </div>
     <div style={{ display:'flex', flexDirection:'column', gap:14 }}>
       {categories.map(function(cat) {
         return (
           <div key={cat.title} style={{ display:'flex', alignItems:'center', gap:16 }}>
             <div style={{ display:'flex', fontSize:10, fontWeight:700, color:cat.color, letterSpacing:'1px', width:80 }}>
               {cat.title.toUpperCase()}
             </div>
             <div style={{ display:'flex', flexWrap:'wrap', gap:7 }}>
               {cat.items.map(function(item) {
                 return (
                   <div key={item} style={{
                     display:'flex', padding:'4px 13px', borderRadius:6,
                     background:cat.color + '15', border:'1px solid ' + cat.color + '35',
                     color:'rgba(225,220,255,0.85)', fontSize:12, fontWeight:600,
                   }}>{item}</div>
                 );
               })}
             </div>
           </div>
         );
       })}
     </div>
   </div>
 );
})()
```

<br/>
<h4 align="center">Cloud, Infrastructure & DB</h4>

```aura width=110 height=44 inline align=center
<SocialMediaButton icon="https://cdn.simpleicons.org/mongodb/47A248" text="MongoDB" backgroundColor="#122912" textColor="#ffffff" width={110} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#122912' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#47A248' }, { offset: '65%', color: '#122912' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
```aura width=100 height=44 inline
<SocialMediaButton icon="https://cdn.simpleicons.org/mysql/4479A1" text="MySQL" backgroundColor="#111e28" textColor="#ffffff" width={100} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#111e28' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#4479A1' }, { offset: '65%', color: '#111e28' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
```aura width=110 height=44 inline
<SocialMediaButton icon="https://cdn.simpleicons.org/docker/2496ED" text="Docker" backgroundColor="#071e2f" textColor="#ffffff" width={110} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#071e2f' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#2496ED' }, { offset: '65%', color: '#071e2f' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
```aura width=130 height=44 inline
<SocialMediaButton icon="https://cdn.simpleicons.org/kubernetes/326CE5" text="Kubernetes" backgroundColor="#0a152e" textColor="#ffffff" width={130} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#0a152e' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#326CE5' }, { offset: '65%', color: '#0a152e' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
```aura width=140 height=44 inline
<SocialMediaButton icon="https://cdn.simpleicons.org/cloudflare/F38020" text="Cloudflare" backgroundColor="#3d2008" textColor="#ffffff" width={140} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#3d2008' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#F38020' }, { offset: '65%', color: '#3d2008' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```

<h4 align="center">Tools</h4>

```aura width=100 height=44 inline align=center
<SocialMediaButton icon="https://cdn.simpleicons.org/git/F05032" text="Git" backgroundColor="#3c140d" textColor="#ffffff" width={100} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#3c140d' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#F05032' }, { offset: '65%', color: '#3c140d' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
```aura width=100 height=44 inline
<SocialMediaButton icon="https://cdn.simpleicons.org/linux/FCC624" text="Linux" backgroundColor="#3f3209" textColor="#ffffff" width={100} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#3f3209' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#FCC624' }, { offset: '65%', color: '#3f3209' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
```aura width=100 height=44 inline
<SocialMediaButton icon="https://cdn.simpleicons.org/ubuntu/E95420" text="Ubuntu" backgroundColor="#3a1508" textColor="#ffffff" width={100} height={44} gradientStops={[{ offset: '0%', color: '#ffffff' }, { offset: '15%', color: '#3a1508' }, { offset: '30%', color: '#cccccc' }, { offset: '50%', color: '#E95420' }, { offset: '65%', color: '#3a1508' }, { offset: '80%', color: '#888888' }, { offset: '100%', color: '#444444' }]} iconSize={22} />
```
</div>

---

## ⏳ Experience & Journey

- **2026** — M.Tech CS at Indian Statistical Institute (ISI) 
- **2025** — Research Internship at Indian Statistical Institute (ISI) | Planetary Material Prediction | Medical Image Registration Research
- **2024** — Backend Engineering at TechnoHacks & CodeSoft
- **2023** — Active Open Source Contributions (Hacktoberfest '23 & '24)
- **2022** — Began Open Source Journey & Competitive Programming

---

<div align="center">

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Hand%20gestures/Handshake.png" alt="Handshake" width="35" height="35" /> Let's Connect

**[Explore My Portfolio](https://swarnabha.tech/) • [Connect on LinkedIn](https://linkedin.com/in/swarnabha-halder-627692254)**

<br><br>

<a href="https://github.com/piyushsuthar/github-readme-quotes">
  <img src="https://quotes-github-readme.vercel.app/api?type=horizontal&theme=tokyonight" alt="Dynamic Programming Quote" />
</a>

<br>
<p align="center"><sub>𝗉𝗈𝗐𝖾𝗋𝖾𝖽 𝖻𝗒 <a href="https://github.com/collectioneur/readme-aura">𝗋𝖾𝖺𝖽𝗆𝖾-𝖺𝗎𝗋𝖺</a></sub></p>
</div>
