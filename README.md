
<style>
@import url('https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&family=Syne:wght@400;500;700;800&display=swap');

*{box-sizing:border-box;margin:0;padding:0}
.wrap{font-family:'Syne',sans-serif;color:var(--color-text-primary);max-width:780px;margin:0 auto;padding:2rem 1.5rem}

.hero{display:grid;grid-template-columns:1fr auto;gap:2rem;align-items:start;padding:2.5rem 0 2rem;border-bottom:0.5px solid var(--color-border-tertiary)}
.hero-name{font-size:clamp(2rem,5vw,3.2rem);font-weight:800;line-height:1.05;letter-spacing:-1px}
.hero-name span{color:#1D9E75}
.hero-role{font-family:'Space Mono',monospace;font-size:13px;color:var(--color-text-secondary);margin-top:.5rem;letter-spacing:.05em}
.hero-desc{font-size:15px;color:var(--color-text-secondary);line-height:1.7;margin-top:1rem;max-width:480px}
.avatar-box{width:80px;height:80px;border-radius:16px;background:linear-gradient(135deg,#1D9E75,#0F6E56);display:flex;align-items:center;justify-content:center;font-size:28px;font-weight:800;color:#E1F5EE;letter-spacing:-1px;flex-shrink:0}

.links{display:flex;flex-wrap:wrap;gap:8px;margin-top:1.25rem}
.link-btn{display:inline-flex;align-items:center;gap:6px;font-family:'Space Mono',monospace;font-size:11px;padding:6px 12px;border-radius:20px;text-decoration:none;border:0.5px solid var(--color-border-secondary);color:var(--color-text-secondary);transition:all .15s ease}
.link-btn:hover{background:var(--color-background-secondary);color:var(--color-text-primary);border-color:var(--color-border-primary)}
.link-btn i{font-size:14px}

.section{padding:2rem 0;border-bottom:0.5px solid var(--color-border-tertiary)}
.section:last-child{border-bottom:none}
.sec-label{font-family:'Space Mono',monospace;font-size:10px;letter-spacing:.15em;text-transform:uppercase;color:#1D9E75;margin-bottom:1.25rem;display:flex;align-items:center;gap:8px}
.sec-label::after{content:'';flex:1;height:0.5px;background:var(--color-border-tertiary)}

.about-grid{display:grid;grid-template-columns:1fr 1fr;gap:12px}
.about-card{background:var(--color-background-secondary);border-radius:10px;padding:14px 16px}
.about-card .label{font-size:11px;color:var(--color-text-tertiary);margin-bottom:4px;font-family:'Space Mono',monospace}
.about-card .val{font-size:14px;font-weight:500}

.stack-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(130px,1fr));gap:8px}
.tag{background:var(--color-background-secondary);border:0.5px solid var(--color-border-tertiary);border-radius:8px;padding:8px 12px;font-size:13px;font-weight:500;display:flex;align-items:center;gap:8px;transition:border-color .15s}
.tag:hover{border-color:var(--color-border-primary)}
.tag-dot{width:7px;height:7px;border-radius:50%;flex-shrink:0}
.dot-green{background:#1D9E75}
.dot-orange{background:#EF9F27}
.dot-blue{background:#378ADD}
.dot-purple{background:#7F77DD}
.dot-coral{background:#D85A30}

.projects{display:flex;flex-direction:column;gap:16px}
.proj-card{background:var(--color-background-primary);border:0.5px solid var(--color-border-tertiary);border-radius:14px;padding:1.25rem 1.5rem;transition:border-color .2s,transform .2s;cursor:default;position:relative;overflow:hidden}
.proj-card::before{content:'';position:absolute;top:0;left:0;width:3px;height:100%;border-radius:4px 0 0 4px}
.proj-card.green::before{background:#1D9E75}
.proj-card.amber::before{background:#EF9F27}
.proj-card.blue::before{background:#378ADD}
.proj-card:hover{border-color:var(--color-border-primary);transform:translateX(3px)}
.proj-header{display:flex;justify-content:space-between;align-items:flex-start;gap:1rem;margin-bottom:.75rem}
.proj-name{font-size:17px;font-weight:700}
.proj-link{font-family:'Space Mono',monospace;font-size:11px;color:#1D9E75;text-decoration:none;display:flex;align-items:center;gap:4px;white-space:nowrap;flex-shrink:0}
.proj-link:hover{text-decoration:underline}
.proj-desc{font-size:13px;color:var(--color-text-secondary);line-height:1.65;margin-bottom:1rem}
.proj-tags{display:flex;flex-wrap:wrap;gap:6px}
.ptag{font-family:'Space Mono',monospace;font-size:10px;padding:3px 8px;border-radius:4px;background:var(--color-background-secondary);color:var(--color-text-secondary);border:0.5px solid var(--color-border-tertiary)}

.skills-cols{display:grid;grid-template-columns:1fr 1fr;gap:2rem}
.skill-group h4{font-size:12px;font-family:'Space Mono',monospace;letter-spacing:.1em;color:var(--color-text-tertiary);text-transform:uppercase;margin-bottom:.75rem}
.skill-item{display:flex;justify-content:space-between;align-items:center;padding:8px 0;border-bottom:0.5px solid var(--color-border-tertiary)}
.skill-item:last-child{border-bottom:none}
.skill-name{font-size:14px}
.skill-bar{width:80px;height:4px;background:var(--color-background-secondary);border-radius:2px;overflow:hidden}
.skill-fill{height:100%;border-radius:2px;background:#1D9E75;transition:width .4s ease}

.certs-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:10px}
.cert-card{background:var(--color-background-secondary);border-radius:10px;padding:14px 16px;display:flex;flex-direction:column;gap:6px}
.cert-org{font-size:11px;font-family:'Space Mono',monospace;color:var(--color-text-tertiary)}
.cert-name{font-size:13px;font-weight:600;line-height:1.35}
.cert-link{font-size:11px;color:#1D9E75;text-decoration:none;display:flex;align-items:center;gap:4px;margin-top:2px}
.cert-link:hover{text-decoration:underline}

.learning-list{display:flex;flex-direction:column;gap:8px}
.learn-item{display:flex;align-items:center;gap:12px;padding:12px 16px;background:var(--color-background-secondary);border-radius:10px;font-size:14px}
.learn-badge{font-family:'Space Mono',monospace;font-size:10px;padding:3px 8px;border-radius:4px;background:#E1F5EE;color:#0F6E56;white-space:nowrap}

.footer{padding:2rem 0 1rem;text-align:center}
.footer p{font-family:'Space Mono',monospace;font-size:12px;color:var(--color-text-tertiary);font-style:italic}
.footer p span{color:#1D9E75}

@media(max-width:560px){
  .hero{grid-template-columns:1fr}
  .avatar-box{display:none}
  .about-grid{grid-template-columns:1fr}
  .skills-cols{grid-template-columns:1fr}
}
</style>

<div class="wrap">
  <h2 class="sr-only" style="position:absolute;width:1px;height:1px;overflow:hidden">Praful Kadam — Flutter Developer Portfolio</h2>

  <div class="hero">
    <div>
      <div class="hero-name">Praful<br><span>Kadam.</span></div>
      <div class="hero-role">// Flutter Developer · Mumbai, India</div>
      <div class="hero-desc">Building production-ready mobile &amp; web apps with clean UI, real-time systems, and offline-first architectures.</div>
      <div class="links">
        <a class="link-btn" href="https://linkedin.com/in/prafulkadam"><i class="ti ti-brand-linkedin" aria-hidden="true"></i>LinkedIn</a>
        <a class="link-btn" href="https://github.com/Praful2604"><i class="ti ti-brand-github" aria-hidden="true"></i>GitHub</a>
        <a class="link-btn" href="mailto:prafulkadam8697@gmail.com"><i class="ti ti-mail" aria-hidden="true"></i>Email</a>
        <a class="link-btn" href="https://drive.google.com/file/d/1YebQRKNXg5DvjdErwsKpN6ct9hOaIToL/view?usp=drive_link"><i class="ti ti-file-cv" aria-hidden="true"></i>Resume</a>
      </div>
    </div>
    <div class="avatar-box">PK</div>
  </div>

  <div class="section">
    <div class="sec-label">About</div>
    <div class="about-grid">
      <div class="about-card"><div class="label">Status</div><div class="val">Open to Flutter roles &amp; freelance</div></div>
      <div class="about-card"><div class="label">Education</div><div class="val">B.E. Computer Engineering · June 2026</div></div>
      <div class="about-card"><div class="label">Location</div><div class="val">Mumbai, Maharashtra, India</div></div>
      <div class="about-card"><div class="label">Interests</div><div class="val">Scalable architecture · Real-time systems</div></div>
    </div>
  </div>

  <div class="section">
    <div class="sec-label">Tech Stack</div>
    <div class="stack-grid">
      <div class="tag"><span class="tag-dot dot-blue"></span>Flutter / Dart</div>
      <div class="tag"><span class="tag-dot dot-green"></span>Firebase</div>
      <div class="tag"><span class="tag-dot dot-green"></span>Supabase</div>
      <div class="tag"><span class="tag-dot dot-blue"></span>Provider</div>
      <div class="tag"><span class="tag-dot dot-orange"></span>Riverpod</div>
      <div class="tag"><span class="tag-dot dot-orange"></span>BLoC</div>
      <div class="tag"><span class="tag-dot dot-purple"></span>Isar / Hive</div>
      <div class="tag"><span class="tag-dot dot-purple"></span>SQLite</div>
      <div class="tag"><span class="tag-dot dot-coral"></span>REST / Dio</div>
      <div class="tag"><span class="tag-dot dot-blue"></span>HTML5 / CSS3</div>
      <div class="tag"><span class="tag-dot dot-green"></span>Git / GitHub</div>
      <div class="tag"><span class="tag-dot dot-orange"></span>Figma</div>
    </div>
  </div>

  <div class="section">
    <div class="sec-label">Featured Projects</div>
    <div class="projects">
      <div class="proj-card green">
        <div class="proj-header">
          <div class="proj-name">Feedback Flow</div>
          <a class="proj-link" href="https://github.com/Praful2604/feedback_flow_Student_app"><i class="ti ti-external-link" aria-hidden="true"></i>View repo</a>
        </div>
        <div class="proj-desc">Role-based complaint management platform with real-time Firestore listeners, anonymous submission support, and an admin dashboard for resolution tracking.</div>
        <div class="proj-tags">
          <span class="ptag">Firebase Auth</span>
          <span class="ptag">Firestore</span>
          <span class="ptag">RBAC</span>
          <span class="ptag">Real-time</span>
        </div>
      </div>
      <div class="proj-card amber">
        <div class="proj-header">
          <div class="proj-name">Instant Photos</div>
          <a class="proj-link" href="https://github.com/Praful2604/instant-photos-website"><i class="ti ti-external-link" aria-hidden="true"></i>View repo</a>
        </div>
        <div class="proj-desc">Cloud photo sharing platform with face recognition–based filtering, real-time photo updates via Firebase Storage, and event-based album management on mobile and web.</div>
        <div class="proj-tags">
          <span class="ptag">Face Recognition</span>
          <span class="ptag">Firebase Storage</span>
          <span class="ptag">Flutter Web</span>
        </div>
      </div>
      <div class="proj-card blue">
        <div class="proj-header">
          <div class="proj-name">SevaSutra</div>
          <a class="proj-link" href="https://github.com/Praful2604/SevaSutra"><i class="ti ti-external-link" aria-hidden="true"></i>View repo</a>
        </div>
        <div class="proj-desc">Offline-first community health survey app using Isar DB for local persistence with automatic Firestore sync on reconnect, dynamic form builder, and local health analytics.</div>
        <div class="proj-tags">
          <span class="ptag">Isar DB</span>
          <span class="ptag">Offline-first</span>
          <span class="ptag">Auto-sync</span>
          <span class="ptag">Data viz</span>
        </div>
      </div>
    </div>
  </div>

  <div class="section">
    <div class="sec-label">Skills</div>
    <div class="skills-cols">
      <div class="skill-group">
        <h4>Core</h4>
        <div class="skill-item"><span class="skill-name">Flutter / Dart</span><div class="skill-bar"><div class="skill-fill" style="width:90%"></div></div></div>
        <div class="skill-item"><span class="skill-name">Firebase</span><div class="skill-bar"><div class="skill-fill" style="width:85%"></div></div></div>
        <div class="skill-item"><span class="skill-name">Provider</span><div class="skill-bar"><div class="skill-fill" style="width:80%"></div></div></div>
        <div class="skill-item"><span class="skill-name">REST / Dio</span><div class="skill-bar"><div class="skill-fill" style="width:78%"></div></div></div>
        <div class="skill-item"><span class="skill-name">Git</span><div class="skill-bar"><div class="skill-fill" style="width:82%"></div></div></div>
      </div>
      <div class="skill-group">
        <h4>Learning</h4>
        <div class="skill-item"><span class="skill-name">Riverpod</span><div class="skill-bar"><div class="skill-fill" style="width:50%;background:#EF9F27"></div></div></div>
        <div class="skill-item"><span class="skill-name">BLoC Pattern</span><div class="skill-bar"><div class="skill-fill" style="width:45%;background:#EF9F27"></div></div></div>
        <div class="skill-item"><span class="skill-name">CI/CD (Fastlane)</span><div class="skill-bar"><div class="skill-fill" style="width:40%;background:#EF9F27"></div></div></div>
        <div class="skill-item"><span class="skill-name">Clean Architecture</span><div class="skill-bar"><div class="skill-fill" style="width:55%;background:#EF9F27"></div></div></div>
        <div class="skill-item"><span class="skill-name">Supabase</span><div class="skill-bar"><div class="skill-fill" style="width:60%"></div></div></div>
      </div>
    </div>
  </div>

  <div class="section">
    <div class="sec-label">Certifications</div>
    <div class="certs-grid">
      <div class="cert-card">
        <div class="cert-org">Udemy</div>
        <div class="cert-name">Advanced Flutter Development</div>
        <a class="cert-link" href="https://drive.google.com/file/d/1kKXq2sTUpW8anFELbsrFI1-axk6IJQOO/view"><i class="ti ti-external-link" style="font-size:12px" aria-hidden="true"></i>View certificate</a>
      </div>
      <div class="cert-card">
        <div class="cert-org">LinkedIn Learning</div>
        <div class="cert-name">Flutter Essential Training</div>
        <a class="cert-link" href="https://drive.google.com/file/d/15gpZzkpkGnScVFfQ5VuLK_IcFeKl76RM/view"><i class="ti ti-external-link" style="font-size:12px" aria-hidden="true"></i>View certificate</a>
      </div>
      <div class="cert-card">
        <div class="cert-org">LinkedIn Learning</div>
        <div class="cert-name">Firebase Essential Training</div>
        <a class="cert-link" href="https://drive.google.com/file/d/1KGrUls5dMDwjNeTiEPt5nDXgsBwxmt7V/view"><i class="ti ti-external-link" style="font-size:12px" aria-hidden="true"></i>View certificate</a>
      </div>
      <div class="cert-card">
        <div class="cert-org">Anthropic</div>
        <div class="cert-name">Claude 101</div>
        <a class="cert-link" href="https://drive.google.com/file/d/1c1tQlJQ55ESClzGiOm6TFJFGQT__rNJ3/view"><i class="ti ti-external-link" style="font-size:12px" aria-hidden="true"></i>View certificate</a>
      </div>
    </div>
  </div>

  <div class="section">
    <div class="sec-label">Currently Learning</div>
    <div class="learning-list">
      <div class="learn-item"><i class="ti ti-wave-square" style="color:#1D9E75;font-size:18px" aria-hidden="true"></i>Riverpod — reactive state management for scalable Flutter apps<span class="learn-badge" style="margin-left:auto">In progress</span></div>
      <div class="learn-item"><i class="ti ti-stack" style="color:#378ADD;font-size:18px" aria-hidden="true"></i>BLoC Pattern — predictable state with clean separation<span class="learn-badge" style="margin-left:auto;background:#E6F1FB;color:#185FA5">In progress</span></div>
      <div class="learn-item"><i class="ti ti-git-branch" style="color:#EF9F27;font-size:18px" aria-hidden="true"></i>CI/CD — GitHub Actions &amp; Fastlane for Flutter deployments<span class="learn-badge" style="margin-left:auto;background:#FAEEDA;color:#854F0B">In progress</span></div>
      <div class="learn-item"><i class="ti ti-building" style="color:#7F77DD;font-size:18px" aria-hidden="true"></i>Clean Architecture — long-term app maintainability patterns<span class="learn-badge" style="margin-left:auto;background:#EEEDFE;color:#534AB7">In progress</span></div>
    </div>
  </div>

  <div class="footer">
    <p>"First, solve the problem. Then, write the code."<br><br><span>prafulkadam8697@gmail.com</span> · +91 8087614598</p>
  </div>
</div>
