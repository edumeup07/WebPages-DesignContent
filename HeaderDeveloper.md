# Header UI – Developer Specification

Document version: 1.1  
Last updated: January 27, 2026  
Scope: Responsive header with mega menu, dropdowns, CTAs, and mobile overlay per header.txt.

---

## 1) HTML Structure
```html
<header class="site-header" role="banner">
  <div class="header__inner">
    <a class="header__logo" href="/" aria-label="EduMeUp Home">
      <img src="/images/logos/edumeup-logo.svg" alt="EduMeUp" width="180" height="40">
    </a>

    <nav class="header__nav" aria-label="Main navigation">
      <ul class="header__nav-list">
        <li class="has-mega">
          <button class="nav__trigger" aria-expanded="false" aria-controls="mega-start">Start Study ▾</button>
          <div id="mega-start" class="mega" hidden>
            <div class="mega__col mega__col--wide">
              <h3>Choose by Grade Level</h3>
              <ul>
                <li><a href="/starter-primary">🎨 Starter Primary <span>Play-based foundational learning</span></a></li>
                <li><a href="/lower-primary">📚 Lower Primary <span>Reading fluency & problem solving</span></a></li>
                <li><a href="/upper-primary">🔬 Upper Primary <span>Abstract thinking & scientific reasoning</span></a></li>
                <li class="is-featured"><a href="/get-ready">🎯 Get Ready <span>World's only O-Level bridge program</span><em>⭐ UNIQUE</em></a></li>
                <li><a href="/olevel-igcse">🎓 O-Level / IGCSE <span>Complete Cambridge curriculum</span></a></li>
                <li><a href="/fsc-intermediate">🏛️ FSc / Intermediate <span>Pakistan Board + MDCAT/ECAT</span></a></li>
              </ul>
            </div>
            <div class="mega__col">
              <h3>Browse by Subject</h3>
              <ul>
                <li><a href="/subjects/mathematics">Σ Mathematics <span>Grade 1 - O-Level</span></a></li>
                <li><a href="/subjects/english">📖 English <span>Literacy & Language</span></a></li>
                <li><a href="/subjects/physics">⚛️ Physics <span>O-Level Physics</span></a></li>
                <li><a href="/subjects/chemistry">🧪 Chemistry <span>O-Level Chemistry</span></a></li>
                <li><a href="/subjects/biology">🧬 Biology <span>O-Level Biology</span></a></li>
                <li><a class="mega__link-cta" href="/courses">View All Subjects →</a></li>
              </ul>
            </div>
            <div class="mega__col">
              <div class="mega__feature">
                <div class="badge">⭐ FEATURED</div>
                <h3>Get Ready Courses</h3>
                <p>92% O-Level pass rate (vs 55% without)</p>
                <a class="btn btn--secondary" href="/get-ready">Discover Get Ready →</a>
              </div>
              <div class="mega__quick">
                <h4>Quick Start</h4>
                <ul>
                  <li><a href="/diagnostic">Take Free Diagnostic Test</a></li>
                  <li><a href="/courses">Browse All Courses</a></li>
                  <li><a href="/sample-lessons">See Sample Lessons</a></li>
                  <li><a href="/pricing">View Pricing</a></li>
                </ul>
              </div>
            </div>
          </div>
        </li>

        <li class="has-dropdown">
          <button class="nav__trigger" aria-expanded="false" aria-controls="dd-serve">Who We Serve ▾</button>
          <div id="dd-serve" class="dropdown" hidden>
            <a href="/students">🎓 For Students <span>Self-paced mastery learning</span></a>
            <a href="/parents">👨‍👩‍👧 For Parents <span>Real-time visibility & control</span></a>
            <a href="/homeschool">🏡 For Homeschool Families <span>Complete curriculum + validation</span></a>
            <a href="/teachers">👨‍🏫 For Teachers <span>Ready-made resources + income</span></a>
            <a href="/schools">🏫 For Schools <span>Institutional solutions</span></a>
            <div class="dropdown__divider"></div>
            <a class="dropdown__cta" href="/compare">Compare Solutions →</a>
          </div>
        </li>

        <li class="has-dropdown">
          <button class="nav__trigger" aria-expanded="false" aria-controls="dd-about">About ▾</button>
          <div id="dd-about" class="dropdown" hidden>
            <a href="/about">📖 Our Story <span>Mission, vision, and values</span></a>
            <a href="/how-it-works">⚙️ How It Works <span>Platform features explained</span></a>
            <a href="/research" class="has-badge">🔬 Research & Validation <em>UNIVERSITY-PROVEN</em><span>Independent university study</span></a>
            <a href="/team">👥 Our Team <span>Meet the educators & experts</span></a>
            <a href="/success-stories">🏆 Success Stories <span>Real students, real results</span></a>
            <div class="dropdown__divider"></div>
            <a class="dropdown__cta" href="/why-edumeup">Why Choose EduMeUp? →</a>
          </div>
        </li>

        <li class="has-dropdown">
          <button class="nav__trigger" aria-expanded="false" aria-controls="dd-resources">Resources ▾</button>
          <div id="dd-resources" class="dropdown dropdown--sectioned" hidden>
            <div class="dropdown__section">
              <h4>Learning Resources</h4>
              <a href="/blog">📝 Blog <span>Education tips & insights</span></a>
              <a href="/sample-lessons">🎬 Sample Lessons <span>Try before you enroll</span></a>
              <a href="/past-papers">📄 Past Papers Library <span>Enhanced O-Level papers</span></a>
              <a href="/parent-guide">📚 Parent Guide <span>Support your child's learning</span></a>
            </div>
            <div class="dropdown__divider"></div>
            <div class="dropdown__section">
              <h4>Support</h4>
              <a href="/help">❓ Help Center <span>FAQs & troubleshooting</span></a>
              <a href="/contact">💬 Contact Us <span>Get in touch with our team</span></a>
              <a href="/demo">📅 Schedule Demo <span>Book a live walkthrough</span></a>
            </div>
          </div>
        </li>

        <li><a href="/pricing">Pricing</a></li>
      </ul>
    </nav>

    <div class="header__cta">
      <a class="btn btn--outline" href="/my-account">My Account</a>
      <a class="btn btn--primary" href="/diagnostic">Start Diagnostic →</a>
    </div>

    <button class="header__hamburger" aria-label="Open menu" aria-expanded="false" aria-controls="mobile-menu">
      <span class="hamburger__bar"></span>
      <span class="hamburger__bar"></span>
      <span class="hamburger__bar"></span>
    </button>
  </div>

  <div id="mobile-menu" class="mobile-menu" hidden>
    <div class="mobile-menu__header">
      <span class="mobile-menu__logo">EduMeUp</span>
      <button class="mobile-menu__close" aria-label="Close menu">×</button>
    </div>
    <div class="mobile-menu__body">
      <section>
        <h4>Start Study</h4>
        <a href="/starter-primary">Starter Primary</a>
        <a href="/lower-primary">Lower Primary</a>
        <a href="/upper-primary">Upper Primary</a>
        <a href="/get-ready">Get Ready (⭐)</a>
        <a href="/olevel-igcse">O-Level / IGCSE</a>
        <a href="/fsc-intermediate">FSc / Intermediate</a>
        <a href="/courses">All Subjects →</a>
      </section>
      <section>
        <h4>Who We Serve</h4>
        <a href="/students">For Students</a>
        <a href="/parents">For Parents</a>
        <a href="/homeschool">For Homeschool Families</a>
        <a href="/teachers">For Teachers</a>
        <a href="/schools">For Schools</a>
        <a href="/compare">Compare Solutions →</a>
      </section>
      <section>
        <h4>About</h4>
        <a href="/about">Our Story</a>
        <a href="/how-it-works">How It Works</a>
        <a href="/research">Research & Validation</a>
        <a href="/team">Our Team</a>
        <a href="/success-stories">Success Stories</a>
        <a href="/why-edumeup">Why Choose EduMeUp?</a>
      </section>
      <section>
        <h4>Resources</h4>
        <a href="/blog">Blog</a>
        <a href="/sample-lessons">Sample Lessons</a>
        <a href="/past-papers">Past Papers Library</a>
        <a href="/parent-guide">Parent Guide</a>
        <a href="/help">Help Center</a>
        <a href="/contact">Contact Us</a>
        <a href="/demo">Schedule Demo</a>
      </section>
      <a class="mobile-menu__link" href="/pricing">Pricing</a>
      <a class="mobile-menu__link" href="/my-account">My Account</a>
      <a class="btn btn--primary mobile-menu__cta" href="/diagnostic">Start Diagnostic →</a>
    </div>
  </div>
</header>
```

---

## 2) Core CSS (Key Rules)
```css
:root {
  --header-height-desktop: 80px;
  --header-height-tablet: 70px;
  --header-height-mobile: 64px;
  --header-bg: #ffffff;
  --header-text: #1A2B3C;
  --header-hover: #1E40AF;
  --header-border: #E5E7EB;
  --shadow-header: 0 2px 8px rgba(0,0,0,0.06);
}

.site-header { position: sticky; top: 0; z-index: 1000; background: var(--header-bg); box-shadow: var(--shadow-header); }
.header__inner { max-width: 1200px; margin: 0 auto; padding: 0 24px; height: var(--header-height-desktop); display: grid; grid-template-columns: auto 1fr auto auto; align-items: center; gap: 16px; }

.header__nav-list { display: flex; gap: 32px; list-style: none; align-items: center; }
.header__nav a, .nav__trigger { font: 600 15px 'Montserrat', sans-serif; color: var(--header-text); background: none; border: none; padding: 12px 0; cursor: pointer; border-bottom: 2px solid transparent; transition: color 150ms ease, border-color 150ms ease; }
.header__nav a:hover, .nav__trigger:hover { color: var(--header-hover); border-bottom-color: var(--header-hover); }
.header__nav a.is-active { color: var(--header-hover); border-bottom-color: var(--header-hover); }

.header__cta { display: flex; gap: 12px; }
.btn { display: inline-flex; align-items: center; justify-content: center; height: 44px; padding: 0 18px; border-radius: 6px; font: 700 15px 'Montserrat', sans-serif; text-decoration: none; }
.btn--primary { background: #1E40AF; color: #fff; box-shadow: 0 2px 8px rgba(30,64,175,0.3); }
.btn--primary:hover { background: #1E3A8A; transform: translateY(-2px); }
.btn--outline { border: 2px solid #1E40AF; color: #1E40AF; background: transparent; }
.btn--outline:hover { background: #F0F9FF; }

/* Mega menu */
.mega { position: absolute; left: 0; right: 0; margin: 0 auto; max-width: 1200px; padding: 40px; background: #fff; box-shadow: 0 4px 16px rgba(0,0,0,0.12); border-radius: 8px; display: grid; grid-template-columns: 40% 30% 30%; gap: 24px; }
.mega__col h3 { font: 700 18px 'Montserrat'; margin-bottom: 12px; color: #1A2B3C; }
.mega__col ul { list-style: none; display: grid; gap: 8px; }
.mega__col a { display: block; padding: 10px 12px; border-radius: 6px; font: 600 15px 'Open Sans', sans-serif; color: #4A5568; border: 2px solid transparent; }
.mega__col a span { display: block; font: 400 14px 'Open Sans'; color: #718096; }
.mega__col a:hover { border-color: #BFDBFE; background: #F0F9FF; color: #1E40AF; }
.mega__col .is-featured a { border-color: #F59E0B; }
.mega__col .is-featured em { background: #F59E0B; color: #fff; font: 700 12px 'Montserrat'; padding: 2px 6px; border-radius: 4px; margin-left: 8px; }
.mega__feature { background: #F0F9FF; border: 2px solid #BFDBFE; border-radius: 8px; padding: 20px; }
.mega__feature .badge { display: inline-block; background: #F59E0B; color: #fff; font: 700 12px 'Montserrat'; padding: 4px 8px; border-radius: 6px; margin-bottom: 8px; }
.mega__quick ul { list-style: none; display: grid; gap: 6px; }

/* Dropdowns */
.dropdown { position: absolute; width: 280px; background: #fff; box-shadow: 0 4px 12px rgba(0,0,0,0.1); border-radius: 8px; padding: 8px 0; display: grid; }
.dropdown a { padding: 12px 20px; font: 600 15px 'Open Sans'; color: #4A5568; text-decoration: none; display: block; }
.dropdown a span { display: block; font: 400 13px 'Open Sans'; color: #718096; }
.dropdown a:hover { background: #F0F9FF; color: #1E40AF; }
.dropdown__divider { height: 1px; background: #E5E7EB; margin: 8px 0; }
.dropdown__cta { font-weight: 700; color: #1E40AF; }
.dropdown--sectioned h4 { padding: 12px 20px 6px; font: 700 14px 'Montserrat'; color: #1A2B3C; background: #F9FAFB; }

/* Mobile */
.header__hamburger { display: none; width: 44px; height: 44px; border: none; background: transparent; }
.hamburger__bar { width: 24px; height: 2px; background: var(--header-text); margin: 5px auto; transition: transform 200ms ease; }
.mobile-menu { position: fixed; inset: 0; background: #fff; z-index: 2000; display: flex; flex-direction: column; padding: 20px; animation: slideIn 300ms ease-out; }
.mobile-menu__body { overflow-y: auto; display: grid; gap: 16px; padding-bottom: 16px; }
.mobile-menu__body a { display: block; padding: 12px 0; font: 700 16px 'Montserrat'; color: #1A2B3C; border-bottom: 1px solid #E5E7EB; }
.mobile-menu__cta { width: 100%; text-align: center; }

@keyframes slideIn { from { transform: translateX(100%); opacity: 0; } to { transform: translateX(0); opacity: 1; } }

@media (max-width: 1023px) {
  .header__inner { padding: 0 20px; height: var(--header-height-tablet); }
  .header__nav-list { gap: 20px; }
}

@media (max-width: 767px) {
  .header__inner { grid-template-columns: auto 1fr auto; padding: 0 16px; height: var(--header-height-mobile); }
  .header__nav, .header__cta { display: none; }
  .header__hamburger { display: inline-flex; align-items: center; justify-content: center; }
  .mega, .dropdown { display: none !important; }
}
```

---

## 3) JavaScript (Dropdowns, Mega, Mobile)
```javascript
const triggers = document.querySelectorAll('.nav__trigger');
const megaMenus = document.querySelectorAll('.mega, .dropdown');
const hamburger = document.querySelector('.header__hamburger');
const mobileMenu = document.getElementById('mobile-menu');
const closeBtn = mobileMenu?.querySelector('.mobile-menu__close');

// Desktop hover/focus open
triggers.forEach(trigger => {
  const targetId = trigger.getAttribute('aria-controls');
  const target = document.getElementById(targetId);
  if (!target) return;

  const open = () => { target.hidden = false; trigger.setAttribute('aria-expanded','true'); };
  const close = () => { target.hidden = true; trigger.setAttribute('aria-expanded','false'); };

  trigger.addEventListener('mouseenter', open);
  trigger.addEventListener('focus', open);
  trigger.parentElement.addEventListener('mouseleave', close);
  trigger.addEventListener('blur', close);
});

// Mobile menu toggle
function openMenu() { mobileMenu.hidden = false; hamburger.setAttribute('aria-expanded','true'); document.body.style.overflow = 'hidden'; }
function closeMenu() { mobileMenu.hidden = true; hamburger.setAttribute('aria-expanded','false'); document.body.style.overflow = ''; }
hamburger?.addEventListener('click', () => { const expanded = hamburger.getAttribute('aria-expanded') === 'true'; expanded ? closeMenu() : openMenu(); });
closeBtn?.addEventListener('click', closeMenu);
mobileMenu?.addEventListener('click', (e) => { if (e.target.tagName === 'A') closeMenu(); });
window.addEventListener('keydown', (e) => { if (e.key === 'Escape') { closeMenu(); megaMenus.forEach(m => m.hidden = true); triggers.forEach(t => t.setAttribute('aria-expanded','false')); } });

// Active link on scroll (anchors)
const sections = ['hero','programs','services','comparison','research','pricing','faq'];
const allLinks = document.querySelectorAll('.header__nav a, .mobile-menu__body a');
const observer = new IntersectionObserver((entries) => {
  entries.forEach(entry => { if (entry.isIntersecting) setActive(entry.target.id); });
}, { rootMargin: '-40% 0px -50% 0px', threshold: 0.1 });

function setActive(id) {
  allLinks.forEach(link => {
    const href = link.getAttribute('href') || '';
    link.classList.toggle('is-active', href === `#${id}` || href.endsWith(`#${id}`));
  });
}

sections.forEach(id => { const el = document.getElementById(id); if (el) observer.observe(el); });
```

---

## 4) Accessibility
- `role="banner"` on header; nav labelled; dropdown/mega triggers use `aria-expanded` + `aria-controls`.
- Close on Escape; mobile overlay locks scroll; optional focus trap for overlay.
- Focus outline 3px #60A5FA with 2px offset on all interactive elements.
- prefers-reduced-motion: disable slide/hover transforms (set transitions to 0ms).
- Touch targets ≥44px; maintain contrast ≥4.5:1 for text and ≥3:1 for outlines.

---

## 5) Performance
- Inline critical header CSS; defer non-critical JS; no jQuery.
- SVG for logo/icons; avoid webfont icons.
- No layout thrash: rely on CSS sticky; avoid scroll listeners for pinning.
- Mega/dropdowns hidden via `hidden` attr (no reflow-heavy display toggles with inline styles).

---

## 6) Testing Checklist
- Desktop: mega opens on hover/focus; columns align; featured card visible; Start Diagnostic CTA size 180×44.
- Dropdowns: Who We Serve/About/Resources open/close cleanly; divider visible; badges present.
- Tablet: nav fits without wrap; link gap reduced; CTAs still visible.
- Mobile: nav/CTAs hidden; hamburger works; overlay shows all IA; links close overlay; scroll lock active.
- Keyboard: Tab through triggers, open/close with focus; Escape closes menus; focus outline visible.
- Accessibility: Contrast, focus, ARIA on triggers/menus, skip link if present.
- No horizontal scroll at 320px; touch targets ≥44px.
