```aura width=860 height=220
<div style={{
  width:'100%', height:'100%', background:'#060609',
  display:'flex', alignItems:'center',
  fontFamily:'Inter', position:'relative', overflow:'hidden',
  borderRadius:20, border:'1px solid rgba(120,80,255,0.18)'
}}>
  <style>{`
    @keyframes d1{0%,100%{transform:translateX(0)}50%{transform:translateX(300px)}}
    @keyframes d2{0%,100%{transform:translateX(0)}50%{transform:translateX(-200px)}}
    @keyframes d3{0%,100%{transform:translateX(0)}50%{transform:translateX(150px)}}
    #g1{animation:d1 11s ease-in-out infinite}
    #g2{animation:d2 15s ease-in-out infinite}
    #g3{animation:d3 9s ease-in-out infinite}
  `}</style>
  <svg width="860" height="220" style={{position:'absolute',top:0,left:0}}>
    <defs>
      <radialGradient id="rg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(100,30,255,0.65)"/>
        <stop offset="100%" stopColor="rgba(100,30,255,0)"/>
      </radialGradient>
      <radialGradient id="rg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(20,80,255,0.5)"/>
        <stop offset="100%" stopColor="rgba(20,80,255,0)"/>
      </radialGradient>
      <radialGradient id="rg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(0,180,255,0.35)"/>
        <stop offset="100%" stopColor="rgba(0,180,255,0)"/>
      </radialGradient>
    </defs>
    <ellipse id="g1" cx="120" cy="280" rx="320" ry="210" fill="url(#rg1)"/>
    <ellipse id="g2" cx="480" cy="280" rx="280" ry="190" fill="url(#rg2)"/>
    <ellipse id="g3" cx="780" cy="280" rx="220" ry="170" fill="url(#rg3)"/>
  </svg>

  <div style={{
    position:'absolute', left:48, top:56, width:108, height:108,
    borderRadius:54, background:'linear-gradient(135deg,#7c3aed,#2563eb)',
    display:'flex', alignItems:'center', justifyContent:'center'
  }}>
    <img src={github?.user?.avatarUrl ?? 'https://github.com/wthm4n.png'} width={100} height={100} style={{borderRadius:50}}/>
  </div>

  <div style={{display:'flex',flexDirection:'column',marginLeft:184,gap:10,zIndex:10}}>
    <div style={{
      fontSize:42, fontWeight:900, letterSpacing:'-1.5px', lineHeight:1,
      background:'linear-gradient(90deg,#c084fc,#818cf8,#38bdf8)',
      backgroundClip:'text', color:'transparent'
    }}>Hey, I'm Rayan 👋</div>
    <div style={{fontSize:15,color:'rgba(190,180,255,0.8)',fontWeight:400,maxWidth:520}}>
      21 · Self-taught dev · Building AI systems, Discord bots & automation tools
    </div>
    <div style={{display:'flex',gap:8,marginTop:4,flexWrap:'wrap'}}>
      {['AI Engineering','Discord.js','Roblox','Linux','Node.js'].map((t,i)=>(
        <div key={i} style={{
          padding:'4px 13px',borderRadius:20,
          background:'rgba(100,60,255,0.16)',
          border:'1px solid rgba(130,90,255,0.3)',
          color:'rgba(210,200,255,0.9)',fontSize:12,fontWeight:600
        }}>{t}</div>
      ))}
    </div>
  </div>
</div>
```

<br/>

```aura width=860 height=150
<div style={{
  width:'100%', height:'100%', background:'#070710',
  display:'flex', alignItems:'center', justifyContent:'space-around',
  fontFamily:'Inter', borderRadius:16, padding:'0 40px',
  border:'1px solid rgba(100,70,220,0.14)'
}}>
  {[
    { emoji:'🤖', label:'Samita AI', sub:'Personality-driven assistant' },
    { emoji:'🧠', label:'Memory & RAG', sub:'Local LLM architectures' },
    { emoji:'💬', label:'Discord Bots', sub:'Large-scale bot systems' },
    { emoji:'🎮', label:'Roblox Dev', sub:'Luau · AoH Lvl 15,000+' },
    { emoji:'⚡', label:'Automation', sub:'CLI tools & pipelines' },
  ].map((c,i)=>(
    <div key={i} style={{display:'flex',flexDirection:'column',alignItems:'center',gap:6,textAlign:'center'}}>
      <div style={{fontSize:30}}>{c.emoji}</div>
      <div style={{fontSize:13,fontWeight:700,color:'#e0d8ff'}}>{c.label}</div>
      <div style={{fontSize:11,color:'rgba(160,155,210,0.7)'}}>{c.sub}</div>
    </div>
  ))}
</div>
```

---

## 🚀 Currently Building

- 🤖 **Samita** — A personality-driven AI assistant with long-term memory
- 🧠 **RAG Systems** — Semantic search + vector database pipelines
- 🎙️ **Voice AI** — Real-time voice interaction systems
- ⚡ **Automation Tools** — GitHub pipelines, file processing, CLI apps

---

## 🛠 Tech Stack

```aura width=860 height=160
<div style={{
  width:'100%', height:'100%', background:'#07070e',
  display:'flex', flexDirection:'column', justifyContent:'center',
  fontFamily:'Inter', borderRadius:16, padding:'20px 40px', gap:16,
  border:'1px solid rgba(90,60,200,0.13)'
}}>
  {[
    {
      category: 'Languages',
      items: [
        {name:'Python',color:'#facc15'},
        {name:'JavaScript',color:'#f59e0b'},
        {name:'TypeScript',color:'#3b82f6'},
        {name:'Luau',color:'#10b981'},
        {name:'HTML/CSS',color:'#f97316'},
      ]
    },
    {
      category: 'Frameworks & Tools',
      items: [
        {name:'Node.js',color:'#22c55e'},
        {name:'Discord.js',color:'#818cf8'},
        {name:'TailwindCSS',color:'#06b6d4'},
        {name:'Ollama',color:'#a78bfa'},
        {name:'MongoDB',color:'#4ade80'},
        {name:'Git',color:'#fb923c'},
        {name:'Linux',color:'#e2e8f0'},
      ]
    }
  ].map((row, i) => (
    <div key={i} style={{display:'flex',alignItems:'center',gap:12}}>
      <div style={{fontSize:11,fontWeight:700,color:'rgba(160,150,210,0.6)',width:120,flexShrink:0}}>{row.category}</div>
      <div style={{display:'flex',gap:8,flexWrap:'wrap'}}>
        {row.items.map((item,j)=>(
          <div key={j} style={{
            padding:'3px 12px', borderRadius:20,
            background:`${item.color}18`,
            border:`1px solid ${item.color}40`,
            color:item.color, fontSize:12, fontWeight:600
          }}>{item.name}</div>
        ))}
      </div>
    </div>
  ))}
</div>
```

---

## 💡 What Makes Me Different

I didn't follow a traditional CS path. My experience comes from **running communities**, **shipping real products**, and **reverse engineering systems** until they made sense.

Strongest at: Rapid prototyping · System architecture · Automation · Community-driven dev

> *Building things, breaking things, and learning from both.*

---

## 📊 GitHub Stats

```aura width=860 height=110
<div style={{
  width:'100%', height:'100%', background:'#07070e',
  display:'flex', alignItems:'center', justifyContent:'space-around',
  fontFamily:'Inter', borderRadius:16, padding:'0 40px',
  border:'1px solid rgba(90,60,200,0.13)'
}}>
  {[
    { label:'Repos', value: github?.user?.repositories?.totalCount ?? '—', color:'#a78bfa' },
    { label:'Followers', value: github?.user?.followers?.totalCount ?? '—', color:'#60a5fa' },
    { label:'Stars Earned', value: github?.starCount ?? '—', color:'#facc15' },
    { label:'Contributions', value: github?.user?.contributionsCollection?.totalCommitContributions ?? '—', color:'#34d399' },
  ].map((s,i)=>(
    <div key={i} style={{display:'flex',flexDirection:'column',alignItems:'center',gap:4}}>
      <div style={{fontSize:28,fontWeight:900,color:s.color}}>{s.value}</div>
      <div style={{fontSize:12,color:'rgba(170,165,210,0.7)',fontWeight:500}}>{s.label}</div>
    </div>
  ))}
</div>
```

---

## 🌐 Find Me

[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white)](#)
[![Discord](https://img.shields.io/badge/Discord-5865F2?style=for-the-badge&logo=discord&logoColor=white)](#)
[![Twitter](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](#)

---

<div align="center">

*𝔭𝔬𝔴𝔢𝔯𝔢𝔡 𝔟𝔶 [𝔯𝔢𝔞𝔡𝔪𝔢-𝔞𝔲𝔯𝔞](https://github.com/collectioneur/readme-aura)*

</div>