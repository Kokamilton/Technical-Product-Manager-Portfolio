# Technical-Product-Manager-Portfolio
The work behind the title
[Koka_Milton_Portfolio_Website.html](https://github.com/user-attachments/files/25720019/Koka_Milton_Portfolio_Website.html)
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/><meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Koka Milton — Technical Product Manager</title>
<link rel="preconnect" href="https://fonts.googleapis.com"/>
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin/>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;700;900&family=DM+Sans:wght@300;400;500;600&family=DM+Mono:wght@400;500&display=swap" rel="stylesheet"/>
<style>
:root{--navy:#0F2540;--steel:#1E3A5F;--accent:#2E7FBF;--accent2:#4A9FD4;--light:#EBF3FA;--gray:#6B7280;--dark:#111827;--off:#F8FAFC;--rule:#CBD5E0;--white:#ffffff;--amber:#92400E;--amber-bg:#FFFBEB;}
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0;}html{scroll-behavior:smooth;}
body{font-family:'DM Sans',sans-serif;background:var(--white);color:var(--dark);line-height:1.6;overflow-x:hidden;}
nav{position:fixed;top:0;left:0;right:0;z-index:100;background:rgba(15,37,64,0.97);backdrop-filter:blur(8px);display:flex;align-items:center;justify-content:space-between;padding:0 3rem;height:60px;border-bottom:1px solid rgba(255,255,255,0.08);}
.nav-name{font-family:'Playfair Display',serif;font-size:1rem;font-weight:700;color:var(--white);letter-spacing:0.03em;}
.nav-links{display:flex;gap:2rem;}.nav-links a{color:rgba(255,255,255,0.65);text-decoration:none;font-size:0.8rem;font-weight:500;letter-spacing:0.08em;text-transform:uppercase;transition:color 0.2s;}.nav-links a:hover{color:var(--accent2);}
.hero{min-height:100vh;background:var(--navy);display:flex;align-items:center;padding:6rem 3rem 4rem;position:relative;overflow:hidden;}
.hero::before{content:'';position:absolute;inset:0;background:radial-gradient(ellipse 60% 50% at 80% 50%,rgba(46,127,191,0.12) 0%,transparent 70%),radial-gradient(ellipse 40% 60% at 10% 80%,rgba(30,58,95,0.6) 0%,transparent 60%);pointer-events:none;}
.hero-inner{max-width:820px;position:relative;z-index:1;}
.hero-eyebrow{font-family:'DM Mono',monospace;font-size:0.72rem;color:var(--accent2);letter-spacing:0.2em;text-transform:uppercase;margin-bottom:1.5rem;opacity:0;animation:fadeUp 0.6s 0.2s forwards;}
.hero h1{font-family:'Playfair Display',serif;font-size:clamp(3rem,7vw,5.5rem);font-weight:900;color:var(--white);line-height:1.05;margin-bottom:1.5rem;opacity:0;animation:fadeUp 0.7s 0.35s forwards;}
.hero h1 span{color:var(--accent2);}
.hero-desc{font-size:1.05rem;color:rgba(255,255,255,0.7);max-width:580px;line-height:1.75;margin-bottom:2.5rem;opacity:0;animation:fadeUp 0.7s 0.5s forwards;}
.hero-tags{display:flex;flex-wrap:wrap;gap:0.6rem;margin-bottom:3rem;opacity:0;animation:fadeUp 0.7s 0.65s forwards;}
.tag{padding:0.35rem 0.9rem;border:1px solid rgba(46,127,191,0.45);border-radius:2px;font-size:0.75rem;font-weight:500;color:rgba(255,255,255,0.75);letter-spacing:0.04em;background:rgba(46,127,191,0.08);}
.hero-contact{font-size:0.82rem;color:rgba(255,255,255,0.45);opacity:0;animation:fadeUp 0.7s 0.8s forwards;}
.hero-scroll{position:absolute;bottom:2.5rem;left:50%;transform:translateX(-50%);display:flex;flex-direction:column;align-items:center;gap:0.4rem;color:rgba(255,255,255,0.3);font-size:0.7rem;letter-spacing:0.1em;text-transform:uppercase;animation:pulse 2s infinite;}
.hero-scroll::after{content:'';width:1px;height:40px;background:linear-gradient(to bottom,rgba(255,255,255,0.3),transparent);}
.section{padding:6rem 3rem;}.section-inner{max-width:860px;margin:0 auto;}.section-alt{background:var(--off);}
.section-label{font-family:'DM Mono',monospace;font-size:0.68rem;color:var(--accent);letter-spacing:0.2em;text-transform:uppercase;margin-bottom:0.75rem;}
.section-title{font-family:'Playfair Display',serif;font-size:clamp(1.6rem,3.5vw,2.4rem);font-weight:700;color:var(--navy);line-height:1.2;margin-bottom:1.5rem;}
.section-rule{width:48px;height:3px;background:var(--accent);margin-bottom:2rem;}
.about-text{font-size:1.02rem;color:#374151;line-height:1.8;margin-bottom:1.2rem;max-width:720px;}
.expertise-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(230px,1fr));gap:0.8rem;margin-top:2rem;}
.expertise-item{padding:0.75rem 1rem;border:1px solid var(--rule);border-left:3px solid var(--accent);background:var(--white);font-size:0.85rem;font-weight:500;color:var(--dark);transition:border-color 0.2s,box-shadow 0.2s;}
.expertise-item:hover{border-left-color:var(--navy);box-shadow:0 2px 12px rgba(15,37,64,0.08);}
.cs-nav{display:flex;gap:0;margin-bottom:3rem;border-bottom:2px solid var(--rule);}
.cs-tab{padding:0.75rem 1.5rem;font-size:0.8rem;font-weight:600;letter-spacing:0.05em;text-transform:uppercase;color:var(--gray);cursor:pointer;border-bottom:2px solid transparent;margin-bottom:-2px;transition:color 0.2s,border-color 0.2s;user-select:none;}
.cs-tab:hover{color:var(--navy);}.cs-tab.active{color:var(--navy);border-bottom-color:var(--navy);}
.cs-panel{display:none;}.cs-panel.active{display:block;}
.cs-number{font-family:'DM Mono',monospace;font-size:0.7rem;color:var(--accent);letter-spacing:0.15em;font-weight:500;}
.cs-title{font-family:'Playfair Display',serif;font-size:clamp(1.3rem,2.5vw,1.8rem);font-weight:700;color:var(--navy);line-height:1.25;margin-bottom:0.35rem;}
.cs-meta{font-size:0.8rem;color:var(--gray);font-style:italic;margin-bottom:2rem;padding-bottom:1.5rem;border-bottom:1px solid var(--rule);}
.cs-section{margin-bottom:1.5rem;}
.cs-section-label{font-family:'DM Mono',monospace;font-size:0.65rem;letter-spacing:0.18em;text-transform:uppercase;color:var(--accent);font-weight:500;margin-bottom:0.6rem;display:flex;align-items:center;gap:0.6rem;}
.cs-section-label::after{content:'';flex:1;height:1px;background:var(--rule);}
.cs-body{font-size:0.95rem;line-height:1.75;color:#374151;margin-bottom:0.75rem;}
.cs-tension{padding:1rem 1.25rem;border-left:3px solid var(--accent);background:var(--light);font-size:0.95rem;font-style:italic;color:var(--steel);line-height:1.7;margin:1rem 0;}
.cs-list{list-style:none;padding:0;}
.cs-list li{padding:0.4rem 0 0.4rem 1.25rem;position:relative;font-size:0.92rem;color:#374151;line-height:1.65;border-bottom:1px solid rgba(203,213,224,0.4);}
.cs-list li:last-child{border-bottom:none;}
.cs-list li::before{content:'▸';position:absolute;left:0;color:var(--accent);font-size:0.7rem;top:0.55rem;}
.cs-outcome-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(280px,1fr));gap:0.75rem;margin-top:0.5rem;}
.cs-outcome-item{padding:0.75rem 1rem;background:var(--navy);color:rgba(255,255,255,0.88);font-size:0.85rem;line-height:1.5;border-left:3px solid var(--accent2);}
.cs-diff{padding:1rem 1.25rem;background:var(--amber-bg);border-left:3px solid #D97706;font-size:0.92rem;font-style:italic;color:var(--amber);line-height:1.7;}
.metrics-grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(180px,1fr));gap:1rem;margin-top:2rem;}
.metric-card{padding:1.25rem;border:1px solid var(--rule);background:var(--white);text-align:center;transition:transform 0.2s,box-shadow 0.2s;}
.metric-card:hover{transform:translateY(-2px);box-shadow:0 4px 16px rgba(15,37,64,0.1);}
.metric-value{font-family:'Playfair Display',serif;font-size:1.9rem;font-weight:900;color:var(--navy);line-height:1;margin-bottom:0.4rem;}
.metric-label{font-size:0.75rem;color:var(--gray);line-height:1.4;}
.contact-section{background:var(--navy);padding:5rem 3rem;text-align:center;}
.contact-section .section-label{color:var(--accent2);}.contact-section .section-title{color:var(--white);margin-bottom:1rem;}
.contact-desc{color:rgba(255,255,255,0.6);font-size:0.95rem;margin-bottom:2rem;}
.contact-info{display:flex;justify-content:center;flex-wrap:wrap;gap:2rem;}
.contact-item{color:rgba(255,255,255,0.75);font-size:0.9rem;}.contact-item strong{color:var(--white);}
footer{background:#080F18;padding:1.5rem 3rem;text-align:center;font-size:0.75rem;color:rgba(255,255,255,0.25);}
@keyframes fadeUp{from{opacity:0;transform:translateY(20px);}to{opacity:1;transform:translateY(0);}}
@keyframes pulse{0%,100%{opacity:0.3;}50%{opacity:0.7;}}
.reveal{opacity:0;transform:translateY(24px);transition:opacity 0.6s ease,transform 0.6s ease;}
.reveal.visible{opacity:1;transform:none;}
</style>
</head>
<body>
<nav>
  <div class="nav-name">Koka Milton</div>
  <div class="nav-links"><a href="#about">About</a><a href="#case-studies">Case Studies</a><a href="#metrics">Impact</a><a href="#contact">Contact</a></div>
</nav>

<section class="hero">
  <div class="hero-inner">
    <div class="hero-eyebrow">Technical Product Manager · Senior / Staff</div>
    <h1>Koka<br/><span>Milton</span></h1>
    <p class="hero-desc">I build platforms that outlast me. Six years leading enterprise product delivery across FinTech, financial services, and hospitality — with 20+ years of domain depth. I specialize in the decisions that don't have playbooks.</p>
    <div class="hero-tags">
      <span class="tag">API Platform Modernization</span><span class="tag">Enterprise Backend Systems</span>
      <span class="tag">Cross-Functional Leadership</span><span class="tag">SAFe Agile · PI Planning</span>
      <span class="tag">ML / OCR Automation</span><span class="tag">SOX · SOC 2 · CFPB Compliance</span>
      <span class="tag">Vendor & Offshore Governance</span>
    </div>
    <div class="hero-contact">(954) 547-3237 &nbsp;·&nbsp; Orlando, FL &nbsp;·&nbsp; Open to Remote / Hybrid / Relocation</div>
  </div>
  <div class="hero-scroll">scroll</div>
</section>

<section class="section" id="about">
  <div class="section-inner">
    <div class="reveal"><div class="section-label">Introduction</div><h2 class="section-title">The work behind the title</h2><div class="section-rule"></div></div>
    <p class="about-text reveal">I am a Technical Product Manager with 6+ years of PM leadership and 20+ years in financial services, specializing in API platform modernization, backend systems architecture, and large-scale enterprise digital transformation. I have owned product backlogs, led cross-functional teams of 40+ engineers, and delivered regulated platforms across FinTech, hospitality, and financial services — consistently under hard deadlines, regulatory constraints, and architectural complexity that has no playbook.</p>
    <div class="expertise-grid reveal">
      <div class="expertise-item">API Platform Modernization</div><div class="expertise-item">SOAP-to-REST Migration</div>
      <div class="expertise-item">Enterprise Backlog Ownership</div><div class="expertise-item">SAFe Agile · PI Planning</div>
      <div class="expertise-item">ML/OCR Automation</div><div class="expertise-item">Cross-Functional Leadership</div>
      <div class="expertise-item">SOX · SOC 2 · Regulatory</div><div class="expertise-item">Vendor & Offshore Governance</div>
      <div class="expertise-item">OKR / KPI Frameworks</div><div class="expertise-item">JIRA · Confluence · Harness</div>
      <div class="expertise-item">Cloud / AWS / CI-CD</div><div class="expertise-item">Python · SageMaker</div>
    </div>
  </div>
</section>

<section class="section section-alt" id="case-studies">
  <div class="section-inner">
    <div class="reveal"><div class="section-label">Case Studies</div><h2 class="section-title">Three decisions that defined the work</h2><div class="section-rule"></div></div>
    <div class="cs-nav reveal">
      <div class="cs-tab active" onclick="showCS(0)">01 · Disney Launch</div>
      <div class="cs-tab" onclick="showCS(1)">02 · AmEx ACORN</div>
      <div class="cs-tab" onclick="showCS(2)">03 · Disney Operating Model</div>
    </div>

    <!-- CS1 -->
    <div class="cs-panel active" id="cs-0">
      <div class="cs-number">CASE STUDY 01</div>
      <div class="cs-title">Architecting a Launch Under Architectural Conflict</div>
      <div class="cs-meta">Senior Technical Product Manager · The Walt Disney Company · 2024</div>
      <div class="cs-section"><div class="cs-section-label">Context</div>
        <p class="cs-body">National Geographic contracted Disney to launch Lindblad expedition cruises as a net-new Disney Vacation Club point redemption product by December 1st — a hard deadline set before any technical discovery occurred. I was the sole Senior TPM across Disney Experiences Technology &amp; Digital, with 3 studios, no formal operating model, and three platform migrations already in flight.</p>
      </div>
      <div class="cs-section"><div class="cs-section-label">The Real Technical Tension</div>
        <p class="cs-body">What entered intake as "add resort code LEX" concealed a critical architectural conflict: the legacy Points system — the only system capable of processing this integration — was actively being decommissioned. Building into it would entrench a retiring system. The replacement platform was mid-flight with no live products. Lindblad would have to become its first production validation under a deadline that predated this constraint entirely.</p>
        <div class="cs-tension">The tension wasn't the deadline. It was: do you build into a retiring system to protect the hard date, or accelerate a platform that isn't ready and own that risk?</div>
      </div>
      <div class="cs-section"><div class="cs-section-label">Constraints</div>
        <ul class="cs-list">
          <li>December 1st contractual deadline — non-negotiable, external stakeholders</li>
          <li>Legacy Points in active decommissioning — building into it created migration debt and dual-system drift</li>
          <li>New Points platform mid-flight — no prior live products, untested at production load</li>
          <li>August 14th finance deadline surfaced mid-discovery — SAP blackout would trigger SOX constraints with less than 8 business days to act</li>
          <li>Lindblad billing model non-standard (direct external vs. Disney intercompany) — no existing precedent</li>
          <li>All DVC member populations required simultaneous support — no phased rollout option</li>
        </ul>
      </div>
      <div class="cs-section"><div class="cs-section-label">Decision Framework</div>
        <p class="cs-body">I reframed the initiative before writing a single story. The question wasn't "how do we hit December 1st" — it was "what's the minimum viable path that hits the date without creating a worse problem 6 months from now?"</p>
        <p class="cs-body">In the discovery call I ran Splunk log analysis on similar Nat Geo products to validate booking flows and confirm viability on the new platform. Once confirmed, the call was clear: build on the new Points platform. Building into a decommissioning system would create dual-system drift and compliance exposure that would cost far more than accelerating an untested one.</p>
        <p class="cs-body">When the August 14th finance deadline surfaced, I escalated immediately, compressed discovery, and mobilized parallel workstreams across legacy Points, Points rewrite, DVC Sales, and Finance — not sequentially as originally scoped.</p>
      </div>
      <div class="cs-section"><div class="cs-section-label">Tradeoffs Made</div>
        <ul class="cs-list">
          <li><strong>Accepted platform risk to eliminate architectural debt.</strong> Lindblad would be the new platform's first live test. But permanent migration complexity on a retiring system was the worse long-term outcome.</li>
          <li><strong>Bumped lower-priority rewrite items to protect December 1st</strong> — documented with full rationale so leadership had visibility and justification to Senior Leadership.</li>
          <li><strong>Chose dual-system support over phased rollout.</strong> Phased would have been operationally safer but created a member experience gap. We absorbed the coordination complexity to protect consistency.</li>
        </ul>
      </div>
      <div class="cs-section"><div class="cs-section-label">Outcome</div>
        <div class="cs-outcome-grid">
          <div class="cs-outcome-item">December 1st delivered — zero member disruption, no SOX delay</div>
          <div class="cs-outcome-item">First live production validation of the new Points platform</div>
          <div class="cs-outcome-item">Zero system divergence between legacy and new platform post-launch</div>
          <div class="cs-outcome-item">All DVC member populations served simultaneously from day one</div>
        </div>
      </div>
      <div class="cs-section"><div class="cs-section-label">What I'd Do Differently</div>
        <div class="cs-diff">TPM involvement at contract negotiation, not intake. The business committed to December 1st without understanding the architectural constraint. A discovery sprint before signature costs a fraction of a hard deadline that collides with a platform migration nobody knew existed.</div>
      </div>
    </div>

    <!-- CS2 — full rewrite -->
    <div class="cs-panel" id="cs-1">
      <div class="cs-number">CASE STUDY 02</div>
      <div class="cs-title">Converting a Regulatory Deadline into an Enterprise Platform Foundation</div>
      <div class="cs-meta">Product Manager / Product Owner — Ops Metrics &amp; US ACORN Foundation · American Express · 2018–2021</div>
      <div class="cs-section"><div class="cs-section-label">Context</div>
        <p class="cs-body">In 2018, American Express was approaching a non-negotiable CFPB regulatory deadline with a critical architectural problem: the existing ACORN platform had been built for Mexico and Argentina at 140K records. That architecture could not scale to the US at 5.3M accounts — a completely different magnitude. Building in RMS, the legacy platform, was ruled out due to technical debt on a system already earmarked for decommission. The team needed a proven technical foundation for the US build, and the deadline was closing in. I was placed as sole PM on Ops Metrics — the initiative that would become that foundation — with no blueprint, no prior architecture, and no other PM sharing ownership.</p>
      </div>
      <div class="cs-section"><div class="cs-section-label">The Real Technical Tension</div>
        <p class="cs-body">The core tension was not execution speed. It was validation architecture: how do you build and prove a technical foundation fast enough to meet a regulatory deadline, when the product's value depends entirely on whether 19 external agency partners — each with their own systems — can successfully ingest and send back data at every stage of the build? You cannot build first and test later. You have to build and validate simultaneously, with live partners, in both directions, from the very first iteration.</p>
        <div class="cs-tension">The real question: can you run a test-driven, multi-stakeholder co-development process — 19 external partners building simultaneously on their side, bi-directionally — fast enough to meet a CFPB deadline, while ensuring zero defects reach production?</div>
      </div>
      <div class="cs-section"><div class="cs-section-label">Constraints</div>
        <ul class="cs-list">
          <li>CFPB regulatory deadline — non-negotiable, no extension possible</li>
          <li>Existing ACORN architecture (MX/ARG) built for 140K records — could not scale to 5.3M US accounts</li>
          <li>Legacy RMS ruled out — technical debt on a system already earmarked for decommission</li>
          <li>19 external outside agency partners — each had to build simultaneously on their side (ingest AND send-back)</li>
          <li>Bi-directional validation required at every iteration — not build-then-test, but build-and-validate in parallel</li>
          <li>No existing JSON schema, no master data model, no prior US architecture to reference</li>
        </ul>
      </div>
      <div class="cs-section"><div class="cs-section-label">Decision Framework</div>
        <p class="cs-body">Three decisions defined the build:</p>
        <ul class="cs-list">
          <li><strong>Test-driven iterative co-development from iteration one.</strong> From the very first 4 entities, I gave the draft schema to all 19 agency partners immediately. They were co-development partners building simultaneously: ingesting files AmEx was sending AND sending data back. Bugs were fixed, validated jointly, and confirmed working before expanding. 4 entities → tested bi-directionally → confirmed → 6 → 9 → 12.</li>
          <li><strong>Strategic isolation of the 3 fastest partners to accelerate the validation cycle.</strong> A pattern emerged: 3 agencies consistently outperformed the others in turnaround time. I made the call to run separate accelerated test sessions with only those 3 — the validation cycle was being rate-limited by the slowest partners. The 3 strongest served as the advance test cohort while all 19 continued on the broader track.</li>
          <li><strong>Architecture built to outlast the deadline.</strong> I created the 8-byte agencyId unique identifier architecture for all 18 partners and built the master 12-entity schema document as the foundational technical reference for both AmEx engineering and all 19 agency partners — building something stable enough that leadership would choose it as the US ACORN baseline.</li>
        </ul>
      </div>
      <div class="cs-section"><div class="cs-section-label">Tradeoffs Made</div>
        <ul class="cs-list">
          <li><strong>Ran external agency validation from iteration one, not after internal stabilization.</strong> The safer approach — build to stable MVP internally, then introduce partners — would have compressed the agency validation window dangerously close to the deadline. Early external involvement risked surfacing bugs early. That risk was smaller than late validation with no buffer.</li>
          <li><strong>Isolated 3 agencies into an accelerated track without pausing the broader group.</strong> Two coordination workflows simultaneously — real operational complexity. But running all 19 at the same pace would have meant the advance cohort perpetually waiting on the slowest partners.</li>
          <li><strong>Prioritized foundation stability over feature breadth at 12 entities.</strong> 12 was the right stopping point — proven, stable, validated bi-directionally across all 19 partners. Once leadership adopted it as the US ACORN baseline, other PMs added their segments on top, scaling to 40+ entities.</li>
        </ul>
      </div>
      <div class="cs-section"><div class="cs-section-label">Outcome</div>
        <div class="cs-outcome-grid">
          <div class="cs-outcome-item">12-entity JSON MVP proven bi-directionally across all 19 agency partners</div>
          <div class="cs-outcome-item">Foundation adopted as baseline for entire US ACORN platform — 40+ entities, 5.3M accounts</div>
          <div class="cs-outcome-item">CFPB regulatory deadline satisfied — OKR #25 and #43 delivered</div>
          <div class="cs-outcome-item">18 agencies released to production; $30K+ recovered from 300-account pilot</div>
          <div class="cs-outcome-item">$28M multi-year enterprise platform investment enterprise investment enabled (2019 Big Bet Priority 1)</div>
          <div class="cs-outcome-item">A CFPB compliance task became the architectural backbone of an enterprise-wide collections platform</div>
        </div>
      </div>
      <div class="cs-section"><div class="cs-section-label">What I'd Do Differently</div>
        <div class="cs-diff">I would have documented the 3-agency accelerated track decision as a formal decision artifact rather than an operational call made in the moment. It was one of the most consequential sequencing decisions in the build — and it lived only in meeting notes. Significant decisions, even operational ones, deserve decision records with explicit tradeoffs captured.</div>
      </div>
    </div>

    <!-- CS3 -->
    <div class="cs-panel" id="cs-2">
      <div class="cs-number">CASE STUDY 03</div>
      <div class="cs-title">Building a TPM Operating Model While the Plane Was Flying</div>
      <div class="cs-meta">Senior Technical Product Manager · The Walt Disney Company · 2024</div>
      <div class="cs-section"><div class="cs-section-label">Context</div>
        <p class="cs-body">I joined Disney in June 2024 as the sole Senior TPM for Disney Experiences Technology &amp; Digital — inheriting 3 Agile studios (Shield, Skywalker, Codegen), 40+ engineers, 60+ backend applications, and zero product operating model. Backlogs were Scrum Master-managed with no intake process, no dependency tracking, and no cross-studio visibility. Three platform migrations were already in flight. Five global resort properties required uninterrupted availability.</p>
      </div>
      <div class="cs-section"><div class="cs-section-label">The Real Technical Tension</div>
        <p class="cs-body">The tension wasn't whether to build an operating model — it was sequencing. Do you pause delivery to build governance infrastructure, or build governance while keeping delivery running?</p>
        <div class="cs-tension">Pausing would have been cleaner. But these systems serve WDW, DLR, DLP, Aulani, and DVC. There is no maintenance window where you go dark for 6 weeks to fix process. Every day without governance was accumulating delivery risk. Every day I paused delivery to build governance was operational risk to live resort infrastructure. I had to build the plane while flying it.</div>
      </div>
      <div class="cs-section"><div class="cs-section-label">Constraints</div>
        <ul class="cs-list">
          <li>No intake process, prioritization framework, or cross-studio visibility — starting from zero</li>
          <li>3 concurrent platform migrations (RHEL7→AL2, Jenkins→Harness, Java 17) in flight with no centralized tracking</li>
          <li>19-engineer offshore Codegen partnership with no governance or accountability structure</li>
          <li>Continuous production availability required across 5 global resort properties</li>
          <li>Bi-weekly COM release cadence that couldn't slip</li>
          <li>100+ SAST vulnerabilities with no remediation prioritization</li>
        </ul>
      </div>
      <div class="cs-section"><div class="cs-section-label">Decision Framework</div>
        <p class="cs-body">I made a deliberate sequencing decision: stabilize visibility before optimizing velocity. The instinct in a chaotic environment is to impose process immediately. But process without trust creates resistance — and resistance in a team already delivering under pressure creates more chaos.</p>
        <p class="cs-body">First two weeks: I observed, mapped, and asked questions without changing anything. I needed to understand what was actually in flight vs. documented, where real dependencies lived, and which Scrum Masters held the most team influence.</p>
        <p class="cs-body">Then I built a 6-criteria intake scoring framework (Organizational Alignment, Cost Impact, Reach, Urgency, Effort, Category) designed to be team-operable, not TPM-dependent. If scoring required me, the framework would break the moment I was unavailable. The goal: a system teams could run themselves, with me as reviewer not operator.</p>
        <p class="cs-body">For Codegen, I reframed UAC sessions from status reviews to unblocking sessions — structured to surface and resolve impediments in the room. That distinction changed how the offshore team engaged entirely.</p>
      </div>
      <div class="cs-section"><div class="cs-section-label">Tradeoffs Made</div>
        <ul class="cs-list">
          <li><strong>Implemented governance incrementally, not comprehensively.</strong> Deploying all frameworks simultaneously would have overwhelmed teams mid-delivery. Sequenced by risk: intake first, then dependency tracking, then UAC governance.</li>
          <li><strong>Accepted short-term velocity dip in weeks 2–4.</strong> Running ceremonies while building the framework caused a slight dip. The alternative — permanent ad-hoc prioritization — was the worse long-term outcome.</li>
          <li><strong>Designed for institutional durability over personal control.</strong> Team-operable is harder to build but survives absence, reorgs, and leadership changes. I optimized for the system outlasting me.</li>
        </ul>
      </div>
      <div class="cs-section"><div class="cs-section-label">Outcome</div>
        <div class="cs-outcome-grid">
          <div class="cs-outcome-item">100+ story points/sprint consistently from week 6 onward</div>
          <div class="cs-outcome-item">4 consecutive COM releases with zero critical defects</div>
          <div class="cs-outcome-item">30% increase in Codegen offshore delivery velocity</div>
          <div class="cs-outcome-item">99.9% platform availability throughout full modernization</div>
          <div class="cs-outcome-item">100+ SAST vulnerabilities remediated to completion</div>
          <div class="cs-outcome-item">Intake framework still in use after contract ended</div>
        </div>
      </div>
      <div class="cs-section"><div class="cs-section-label">What I'd Do Differently</div>
        <div class="cs-diff">I implemented the operating model but never wrote it down as a unified artifact. It lived across trackers, Confluence pages, and ceremonies — never synthesized into a TPM Playbook. Every time leadership asked how it worked, I explained it verbally. A written playbook accelerates alignment, onboards future TPMs faster, and creates institutional memory that survives departure. The model was right. The documentation lagged. That gap closes earlier next time.</div>
      </div>
    </div>
  </div>
</section>

<section class="section" id="metrics">
  <div class="section-inner">
    <div class="reveal"><div class="section-label">Career Impact</div><h2 class="section-title">The numbers behind the decisions</h2><div class="section-rule"></div></div>
    <div class="metrics-grid reveal">
      <div class="metric-card"><div class="metric-value">60+</div><div class="metric-label">Enterprise backend apps owned at Disney</div></div>
      <div class="metric-card"><div class="metric-value">40+</div><div class="metric-label">Engineers led across 3 studios</div></div>
      <div class="metric-card"><div class="metric-value">$1.4B</div><div class="metric-label">BNY Mellon Corporate Trust portfolio</div></div>
      <div class="metric-card"><div class="metric-value">8M</div><div class="metric-label">US accounts on ACORN platform foundation</div></div>
      <div class="metric-card"><div class="metric-value">19</div><div class="metric-label">Agency partners co-developed with simultaneously</div></div>
      <div class="metric-card"><div class="metric-value">$28M multi-year enterprise platform investment</div><div class="metric-label">Enterprise investment enabled by ACORN foundation</div></div>
      <div class="metric-card"><div class="metric-value">30%</div><div class="metric-label">Offshore delivery velocity increase</div></div>
      <div class="metric-card"><div class="metric-value">99.9%</div><div class="metric-label">Platform availability at Disney</div></div>
      <div class="metric-card"><div class="metric-value">Zero</div><div class="metric-label">Critical defects across 8+ production releases</div></div>
      <div class="metric-card"><div class="metric-value">6</div><div class="metric-label">International markets on ACORN platform</div></div>
    </div>
  </div>
</section>

<section class="contact-section" id="contact">
  <div class="section-label">Get In Touch</div>
  <h2 class="section-title">Open to the right conversation</h2>
  <p class="contact-desc">Available for senior / staff TPM roles. Open to remote, hybrid, or relocation.<br/>FinTech · Enterprise SaaS · API Platforms · Regulated Industries</p>
  <div class="contact-info">
    <div class="contact-item"><strong>(954) 547-3237</strong></div>
    <div class="contact-item">Orlando, FL</div>
    <div class="contact-item">Open to Remote / Hybrid / Relocation</div>
  </div>
</section>
<footer>© 2025 Koka Milton · Technical Product Manager</footer>
<script>
function showCS(idx){document.querySelectorAll('.cs-tab').forEach((t,i)=>t.classList.toggle('active',i===idx));document.querySelectorAll('.cs-panel').forEach((p,i)=>p.classList.toggle('active',i===idx));}
const observer=new IntersectionObserver((e)=>{e.forEach(x=>{if(x.isIntersecting)x.target.classList.add('visible');});},{threshold:0.1,rootMargin:'0px 0px -40px 0px'});
document.querySelectorAll('.reveal').forEach(el=>observer.observe(el));
</script>
</body>
</html>
