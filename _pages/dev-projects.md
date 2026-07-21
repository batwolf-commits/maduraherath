---
layout: page
title: dev projects
permalink: /dev-projects/
nav: true
nav_order: 4
_styles: >
  .dev-card {
    display: flex;
    gap: 1.25rem;
    align-items: center;
    padding: 1.25rem 1.5rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 12px;
    max-width: 640px;
  }
  .dev-card img.app-icon {
    width: 84px;
    height: 84px;
    border-radius: 18px;
    flex-shrink: 0;
  }
  .dev-card h3 { margin: 0 0 .3rem; }
  .dev-card p { margin: 0 0 .9rem; color: var(--global-text-color-light); }
  .dev-btn {
    display: inline-block;
    background: var(--global-theme-color);
    color: #fff !important;
    padding: .5rem 1.1rem;
    border-radius: 8px;
    text-decoration: none !important;
    font-weight: 600;
  }
  .dev-btn:hover { opacity: .9; }
  .dev-links { margin-top: .8rem; font-size: .9rem; }
  .dev-links a { margin-right: 1.1rem; }
  @media (max-width: 576px) {
    .dev-card { flex-direction: column; text-align: center; }
  }
---

<div class="dev-card">
  <img class="app-icon" src="{{ '/assets/img/leftspace-icon.png' | relative_url }}" alt="LeftSpace app icon">
  <div class="dev-body">
    <h3>LeftSpace</h3>
    <p>A safe macOS cleaner for developer caches and everyday junk. It finds the gigabytes hidden in npm, Gradle, Xcode, and app caches, then clears them safely. Trash-first by default, so it never touches your documents.</p>
    <a class="dev-btn" href="https://github.com/madurabhathiya/leftspace/releases/latest">Download for macOS</a>
    <div class="dev-links">
      <a href="https://github.com/madurabhathiya/leftspace">View on GitHub</a>
    </div>
  </div>
</div>
