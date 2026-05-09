```aura width=860 height=200
<div style={{
  width: '860px', height: '200px', background: '#080c0a',
  display: 'flex', alignItems: 'center', fontFamily: 'Inter',
  position: 'relative', overflow: 'hidden', borderRadius: '16px',
  border: '1px solid rgba(33,187,133,0.25)'
}}>
  <svg width="860" height="200" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="g1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(33,187,133,0.55)" />
        <stop offset="60%" stopColor="rgba(20,140,100,0.2)" />
        <stop offset="100%" stopColor="rgba(20,140,100,0)" />
      </radialGradient>
      <radialGradient id="g2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(0,255,150,0.3)" />
        <stop offset="70%" stopColor="rgba(0,200,120,0)" />
      </radialGradient>
      <radialGradient id="g3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(33,187,133,0.4)" />
        <stop offset="70%" stopColor="rgba(33,187,133,0)" />
      </radialGradient>
    </defs>
    <ellipse cx="120" cy="180" rx="280" ry="160" fill="url(#g1)" />
    <ellipse cx="480" cy="220" rx="220" ry="140" fill="url(#g2)" />
    <ellipse cx="780" cy="190" rx="160" ry="130" fill="url(#g3)" />
    <text x="800" y="30" fill="rgba(33,187,133,0.12)" fontSize="11" fontFamily="monospace">01001011</text>
    <text x="20" y="185" fill="rgba(33,187,133,0.08)" fontSize="10" fontFamily="monospace">10110100 01101001</text>
    <text x="600" y="170" fill="rgba(33,187,133,0.1)" fontSize="10" fontFamily="monospace">11010011</text>
  </svg>

  <div style={{
    position: 'absolute', left: '44px', top: '52px', width: '96px', height: '96px',
    borderRadius: '48px',
    background: 'linear-gradient(135deg, #21bb85, #0a3d2a)',
    display: 'flex', alignItems: 'center', justifyContent: 'center',
    border: '2px solid rgba(33,187,133,0.6)'
  }}>
    <img src={github.user.avatarUrl} width="88" height="88" style={{ borderRadius: '44px' }} />
  </div>

  <div style={{ display:'flex', flexDirection:'column', marginLeft:'164px', gap:'8px', zIndex: 10 }}>
    <div style={{
      display:'flex', fontSize:'36px', fontWeight:800,
      color:'#ffffff', letterSpacing:'-1.5px', lineHeight:1
    }}>
      {github.user.name || 'Kushagra Mehta'}
    </div>
    <div style={{
      display:'flex', fontSize:'14px',
      color:'rgba(33,230,160,0.9)', fontWeight:500,
      letterSpacing:'0.5px', fontFamily:'monospace'
    }}>
      {'> AI & Data Science · Mumbai, India'}
    </div>
    <div style={{ display:'flex', gap:'8px', marginTop:'6px' }}>
      {['Python', 'ML/DL', 'Neural Nets', 'Surrogate Modelling'].map(function(tag) {
        return (
          <div key={tag} style={{
            display:'flex', padding:'3px 10px', borderRadius:'20px',
            background:'rgba(33,187,133,0.1)',
            border:'1px solid rgba(33,187,133,0.35)',
            color:'rgba(33,230,160,0.9)',
            fontSize:'11px', fontWeight:600, fontFamily:'monospace'
          }}>{tag}</div>
        );
      })}
    </div>
  </div>

  <div style={{
    position:'absolute', right:'28px', top:'18px',
    display:'flex', flexDirection:'column', gap:'5px',
    fontFamily:'monospace', fontSize:'11px',
    color:'rgba(33,187,133,0.45)'
  }}>
    <div style={{ display:'flex' }}>{'// TSEC · BE AI-DS · 2024-28'}</div>
    <div style={{ display:'flex' }}>{'// R² ≈ 0.96 → ANN distillation'}</div>
    <div style={{ display:'flex' }}>{'// open: internships · research'}</div>
  </div>
</div>
```

```aura width=860 height=240
<div style={{
  width: '860px', height: '240px', background: '#080c0a',
  display: 'flex', fontFamily: 'monospace',
  padding: '28px 40px', borderRadius: '16px',
  border: '1px solid rgba(33,187,133,0.2)',
  position: 'relative', overflow: 'hidden'
}}>
  <svg width="860" height="240" style={{ position:'absolute', top:0, left:0 }}>
    <text x="620" y="220" fill="rgba(33,187,133,0.04)" fontSize="110" fontFamily="monospace" fontWeight="bold">{'</>'}</text>
  </svg>

  <div style={{ display:'flex', flexDirection:'column', gap:'5px', zIndex:10, width:'100%' }}>
    <div style={{ display:'flex', color:'rgba(33,187,133,0.45)', fontSize:'12px', marginBottom:'4px' }}>{'# kushagra_mehta.py'}</div>

    <div style={{ display:'flex', color:'#21bb85', fontSize:'15px', fontWeight:700 }}>{'class KushagraMehta:'}</div>
    <div style={{ display:'flex', color:'#ccc', fontSize:'13px', marginLeft:'24px' }}>{'def __init__(self):'}</div>

    {[
      ['self.university', '"TSEC — AI & Data Science (BE, 2024–28)"'],
      ['self.location  ', '"Mumbai, India"'],
      ['self.focus     ', '["Machine Learning", "Deep Learning", "Surrogate Modelling"]'],
      ['self.best_score', '"R² ≈ 0.96  (ANN on distillation column)"'],
      ['self.open_to   ', '["internships", "research collabs", "side projects"]'],
    ].map(function(row) {
      return (
        <div key={row[0]} style={{ display:'flex', marginLeft:'48px', fontSize:'12px', gap:'6px' }}>
          <span style={{ color:'#5af0b0' }}>{row[0]}</span>
          <span style={{ color:'rgba(200,200,200,0.4)' }}>{'='}</span>
          <span style={{ color:'rgba(255,200,100,0.85)' }}>{row[1]}</span>
        </div>
      );
    })}

    <div style={{ display:'flex', marginTop:'8px', color:'#ccc', fontSize:'13px', marginLeft:'24px' }}>
      {'def say_hi(self):'}
    </div>
    <div style={{ display:'flex', marginLeft:'48px', fontSize:'11px', color:'rgba(180,180,180,0.65)' }}>
      {'print("Building things at the intersection of ML & real-world problems.")'}
    </div>

    <div style={{ display:'flex', marginTop:'8px', gap:'20px', fontSize:'12px' }}>
      <span style={{ color:'rgba(33,187,133,0.6)' }}>{'me = KushagraMehta()'}</span>
      <span style={{ color:'rgba(33,187,133,0.6)' }}>{'me.say_hi()'}</span>
    </div>
  </div>
</div>
```

```aura width=860 height=160
<div style={{
  width: '860px', height: '160px', background: '#080c0a',
  display: 'flex', flexDirection: 'column', fontFamily: 'monospace',
  padding: '22px 40px', borderRadius: '16px',
  border: '1px solid rgba(33,187,133,0.2)', gap: '14px'
}}>
  <div style={{ display:'flex', color:'#21bb85', fontSize:'12px', fontWeight:700, letterSpacing:'2px' }}>
    {'⚡ TECH STACK'}
  </div>

  <div style={{ display:'flex', flexDirection:'column', gap:'10px' }}>
    {[
      { label: '// core ML', tags: ['Python', 'NumPy', 'Pandas', 'Matplotlib', 'Scikit-learn'], opacity: 0.95 },
      { label: '// deep learning', tags: ['TensorFlow', 'Keras', 'CNN', 'RNN', 'Neural Networks'], opacity: 0.7 },
      { label: '// other', tags: ['Jupyter', 'SQL', 'Java', 'JavaScript', 'Next.js'], opacity: 0.45 },
    ].map(function(row) {
      return (
        <div key={row.label} style={{ display:'flex', alignItems:'center', gap:'14px' }}>
          <span style={{ color:'rgba(33,187,133,0.4)', fontSize:'11px', minWidth:'110px' }}>{row.label}</span>
          <div style={{ display:'flex', gap:'7px' }}>
            {row.tags.map(function(t) {
              return (
                <div key={t} style={{
                  display:'flex', padding:'2px 9px', borderRadius:'4px',
                  background:'rgba(33,187,133,0.08)',
                  color:('rgba(33,230,160,' + row.opacity + ')'),
                  fontSize:'11px', fontWeight:600,
                  border:'1px solid rgba(33,187,133,0.2)'
                }}>{t}</div>
              );
            })}
          </div>
        </div>
      );
    })}
  </div>
</div>
```

```aura width=860 height=310
<div style={{
  width: '860px', height: '310px', background: '#080c0a',
  display: 'flex', flexDirection: 'column', fontFamily: 'monospace',
  padding: '22px 40px', borderRadius: '16px',
  border: '1px solid rgba(33,187,133,0.2)', gap: '14px'
}}>
  <div style={{ display:'flex', color:'#21bb85', fontSize:'12px', fontWeight:700, letterSpacing:'2px' }}>
    {'🔬 PROJECTS'}
  </div>

  <div style={{ display:'flex', flexDirection:'column', gap:'10px' }}>
    {[
      {
        name: 'Surrogate Modeling — Binary Distillation Column',
        desc: 'DWSIM simulation (Benzene-Toluene) → ML surrogate. Linear Reg, RF & ANN. R² ≈ 0.96.',
        tags: ['Python', 'DWSIM', 'Scikit-learn', 'ANN'],
        stat: 'R²=0.96'
      },
      {
        name: 'Deep Learning Models · TensorFlow',
        desc: 'CNN for image classification (MNIST, Fashion MNIST). RNN for text gen & sentiment analysis.',
        tags: ['TensorFlow', 'Keras', 'NLTK', 'Python'],
        stat: 'CNN+RNN'
      },
      {
        name: 'Stock Price Movement Predictor',
        desc: 'Random Forest on yFinance data. Rolling indicators + volume features + backtesting.',
        tags: ['Scikit-learn', 'Pandas', 'yFinance'],
        stat: 'RF Classifier'
      },
      {
        name: 'TeleMedPilot · SIH 2025',
        desc: 'Telemedicine platform. Smart India Hackathon 2025.',
        tags: ['Next.js', 'TypeScript'],
        stat: 'Hackathon'
      },
    ].map(function(p) {
      return (
        <div key={p.name} style={{
          display:'flex', alignItems:'flex-start', gap:'12px',
          padding:'7px 12px', borderRadius:'6px',
          background:'rgba(33,187,133,0.03)',
          border:'1px solid rgba(33,187,133,0.1)'
        }}>
          <div style={{ display:'flex', flexDirection:'column', flex:1, gap:'3px' }}>
            <div style={{ display:'flex', justifyContent:'space-between', alignItems:'center' }}>
              <span style={{ color:'#e8fff8', fontSize:'12px', fontWeight:700 }}>{p.name}</span>
              <span style={{
                color:'#21bb85', fontSize:'10px', fontWeight:700,
                padding:'1px 8px', borderRadius:'10px',
                background:'rgba(33,187,133,0.12)',
                border:'1px solid rgba(33,187,133,0.25)'
              }}>{p.stat}</span>
            </div>
            <div style={{ color:'rgba(170,170,170,0.65)', fontSize:'11px' }}>{p.desc}</div>
            <div style={{ display:'flex', gap:'5px', marginTop:'2px' }}>
              {p.tags.map(function(tag) {
                return (
                  <span key={tag} style={{
                    color:'rgba(33,230,160,0.55)', fontSize:'10px',
                    padding:'1px 6px', borderRadius:'3px',
                    background:'rgba(33,187,133,0.06)',
                    border:'1px solid rgba(33,187,133,0.12)'
                  }}>{tag}</span>
                );
              })}
            </div>
          </div>
        </div>
      );
    })}
  </div>
</div>
```

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=kushagra819&show_icons=true&theme=github_dark&hide_border=true&title_color=21bb85&icon_color=21bb85&bg_color=080c0a&text_color=aaffdd" height="160" />
  &nbsp;
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=kushagra819&layout=compact&theme=github_dark&hide_border=true&title_color=21bb85&bg_color=080c0a&text_color=aaffdd&hide=jupyter%20notebook" height="160" />
</p>

<p align="center">
  <img width="95%" src="https://github-readme-activity-graph.vercel.app/graph?username=kushagra819&bg_color=080c0a&color=21bb85&line=21bb85&point=ffffff&hide_border=true" />
</p>

```aura width=860 height=70
<div style={{
  width: '860px', height: '70px', background: '#080c0a',
  display: 'flex', alignItems: 'center', justifyContent: 'space-between',
  fontFamily: 'monospace', padding: '0 40px', borderRadius: '16px',
  border: '1px solid rgba(33,187,133,0.15)'
}}>
  <div style={{ display:'flex', gap:'28px' }}>
    {[
      { label: '// email', val: 'kushagramehta21@gmail.com' },
      { label: '// linkedin', val: 'kushagra-mehta-a86916258' },
      { label: '// loc', val: 'Mumbai · India' },
    ].map(function(item) {
      return (
        <div key={item.label} style={{ display:'flex', flexDirection:'column', gap:'2px' }}>
          <span style={{ color:'rgba(33,187,133,0.4)', fontSize:'10px' }}>{item.label}</span>
          <span style={{ color:'rgba(33,230,160,0.8)', fontSize:'11px', fontWeight:600 }}>{item.val}</span>
        </div>
      );
    })}
  </div>
  <div style={{ color:'rgba(33,187,133,0.2)', fontSize:'10px', fontFamily:'monospace' }}>
    {'kushagra819 · powered by readme-aura · 2026'}
  </div>
</div>
```
