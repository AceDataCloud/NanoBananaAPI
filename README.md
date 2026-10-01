# Nano Banana Image Generation API

Nano Banana AI image generation and editing service.

![Platform](https://img.shields.io/badge/platform-Ace%20Data%20Cloud-0f766e?style=flat-square) ![API](https://img.shields.io/badge/type-AI%20API-2563eb?style=flat-square) ![Docs](https://img.shields.io/badge/docs-online-16a34a?style=flat-square)

![Nano Banana Image Generation](https://cdn.acedata.cloud/knpozx.png/thumb_600x300)

API home page: [Ace Data Cloud - Nano Banana Image Generation](https://platform.acedata.cloud/service/nano-banana)

Keywords: nanobanana-api, ai-image, image-editing, image-generation, rest-api, ai-api, aiimage, AI API, REST API, Developer API, Ace Data Cloud

## Why Use Nano Banana Image Generation on Ace Data Cloud

- Unified developer platform with one API key, billing system, and usage tracking
- Production-ready AI API endpoints served from [https://api.acedata.cloud](https://api.acedata.cloud)
- English integration guides, API references, and service documentation
- Global-ready workflow for developers building chat, image, video, music, and search products

## Overview

<style>
.nb-page * { box-sizing: border-box; }
.nb-page h1, .nb-page h2, .nb-page h3, .nb-page h4, .nb-page h5, .nb-page h6, .nb-page p, .nb-page ul, .nb-page ol, .nb-page li, .nb-page pre, .nb-page blockquote, .nb-page table, .nb-page td, .nb-page th { margin: 0; padding: 0; }
.nb-page {
 -webkit-font-smoothing: antialiased;
 -moz-osx-font-smoothing: grayscale;
 color: var(--el-text-color-primary);
 background: var(--el-bg-color);
 line-height: 1.6;
}
.nb-page a { text-decoration: none; color: inherit; }
.nb-page a:hover { text-decoration: none; }
.nb-page ul { list-style: none; }
.markdown-body .nb-page a { color: inherit !important; text-decoration: none !important; }
.markdown-body .nb-page a:hover { text-decoration: none !important; }
.markdown-body .nb-page a.s-btn-primary,
.markdown-body .nb-page a.price-btn-fill,
.markdown-body .nb-page a.btn-cta-light { color: #ffffff !important; }
.markdown-body .nb-page a.s-btn-secondary { color: var(--el-text-color-primary) !important; }
.markdown-body .nb-page a.price-btn-out { color: var(--el-text-color-primary) !important; }
.markdown-body .nb-page a.btn-cta-ghost { color: #94a3b8 !important; }
.markdown-body .nb-page a.btn-cta-ghost:hover { color: #e2e8f0 !important; }
.markdown-body .nb-page h1, .markdown-body .nb-page h2 { border-bottom: none !important; padding-bottom: 0 !important; }
.s-container { max-width: 1200px; margin: 0 auto; padding: 0 24px; }
.s-container-narrow { max-width: 800px; margin: 0 auto; padding: 0 24px; }
.s-container-wide { max-width: 1100px; margin: 0 auto; padding: 0 32px; }
.s-section { padding: 80px 0; }
.s-section-lg { padding: 100px 0; }
.s-section-sm { padding: 48px 0; }
.s-bg-white { background: var(--el-bg-color); }
.s-bg-gray { background: var(--el-bg-color-page); }
.s-bg-dark { background: #0f172a; color: #f8fafc; }
.s-header { text-align: center; margin-bottom: 64px; }
.s-header h2 {
 font-size: clamp(28px, 4vw, 40px);
 font-weight: 700;
 color: var(--el-text-color-primary);
 letter-spacing: normal;
 margin-bottom: 20px;
 line-height: 1.15;
}
.s-header p {
 font-size: clamp(16px, 2vw, 18px);
 color: var(--el-text-color-regular);
 max-width: 640px;
 margin: 0 auto;
 line-height: 1.6;
}
.s-bg-dark .s-header h2 { color: #f8fafc; }
.s-bg-dark .s-header p { color: var(--el-text-color-secondary); }
.nb-page .s-btn-primary {
 display: inline-flex; align-items: center; gap: 6px;
 padding: 14px 28px;
 background: #4285F4; color: #ffffff !important;
 border-radius: 9999px; font-size: 15px; font-weight: 600;
 transition: background 0.2s, transform 0.15s;
 border: none; cursor: pointer;
 text-decoration: none !important;
}
.nb-page .s-btn-primary:hover { background: #3367D6; transform: translateY(-1px); text-decoration: none !important; }
.nb-page .s-btn-secondary {
 display: inline-flex; align-items: center; gap: 6px;
 padding: 14px 28px;
 background: var(--el-bg-color); color: var(--el-text-color-primary) !important;
 border: 1px solid var(--el-border-color-light);
 border-radius: 9999px; font-size: 15px; font-weight: 600;
 transition: border-color 0.2s, background 0.2s;
 cursor: pointer;
 text-decoration: none !important;
}
.nb-page .s-btn-secondary:hover { background: var(--el-bg-color-page); text-decoration: none !important; }
.nb-hero {
 padding: 100px 0 80px;
 text-align: center;
 background: var(--el-bg-color);
 position: relative;
 overflow: hidden;
}
.nb-hero::before {
 content: '';
 position: absolute;
 top: -200px; left: 50%;
 transform: translateX(-50%);
 width: 900px; height: 500px;
 background: radial-gradient(ellipse, rgba(66, 133, 244, 0.06) 0%, transparent 70%);
 pointer-events: none;
}
.hero-badge {
 display: inline-flex; align-items: center; gap: 8px;
 padding: 6px 16px;
 background: var(--el-bg-color-page); border: 1px solid var(--el-border-color-light);
 border-radius: 9999px; font-size: 13px; font-weight: 600; color: var(--el-text-color-regular);
 margin-bottom: 28px;
}
.hero-badge .badge-dot {
 width: 6px; height: 6px; background: #10b981; border-radius: 50%;
 display: inline-block;
}
.nb-hero h1 {
 font-size: clamp(36px, 5vw, 60px);
 font-weight: 700; line-height: 1.05;
 letter-spacing: normal; color: var(--el-text-color-primary);
 margin-bottom: 20px;
 position: relative;
}
.nb-hero h1 span { color: #4285F4; }
.nb-page .hero-subtitle {
 font-size: clamp(16px, 2vw, 20px);
 color: var(--el-text-color-regular); line-height: 1.6;
 max-width: 620px; margin: 0 auto 56px;
 position: relative;
}
.hero-actions {
 display: flex; gap: 12px; justify-content: center;
 flex-wrap: wrap; margin-bottom: 56px; position: relative;
}
.hero-highlights {
 display: flex; align-items: center; justify-content: center;
 gap: 16px; flex-wrap: wrap; position: relative;
}
.hero-highlights .h-item { font-size: 14px; color: var(--el-text-color-regular); font-weight: 500; }
.hero-highlights .h-div { width: 1px; height: 16px; background: var(--el-border-color-light); }
@media (max-width: 640px) {
 .hero-highlights .h-div { display: none; }
 .hero-highlights { gap: 8px 16px; }
 .hero-actions { flex-direction: column; align-items: center; }
 .hero-actions a { width: 100%; max-width: 280px; justify-content: center; }
}
.nb-stats {
 padding: 48px 0;
 background: var(--el-bg-color-page);
 border-top: 1px solid var(--el-border-color-lighter);
 border-bottom: 1px solid var(--el-border-color-lighter);
}
.stats-grid {
 display: grid; grid-template-columns: repeat(4, 1fr);
 gap: 32px; text-align: center;
}
.stat-icon { font-size: 28px; margin-bottom: 12px; }
.stat-val {
 font-size: clamp(28px, 4vw, 40px);
 font-weight: 700; color: var(--el-text-color-primary);
 letter-spacing: normal; margin-bottom: 4px;
}
.stat-lbl { font-size: 14px; color: var(--el-text-color-secondary); font-weight: 500; }
@media (max-width: 768px) { .stats-grid { grid-template-columns: repeat(2, 1fr); gap: 24px; } }
@media (max-width: 480px) { .stats-grid { grid-template-columns: 1fr; gap: 20px; } }
.features-grid {
 display: grid; grid-template-columns: repeat(3, 1fr); gap: 24px;
}
.feat-card {
 padding: 32px 28px;
 border: none; border-radius: 20px; box-shadow: 0 2px 12px 0 rgba(0,0,0,0.08);
 background: var(--el-bg-color);
 transition: border-color 0.2s, box-shadow 0.2s, transform 0.15s;
}
.feat-card:hover { box-shadow: 0 8px 24px 0 rgba(0,0,0,0.12);
 transform: translateY(-2px);
}
.feat-icon { font-size: 32px; margin-bottom: 16px; }
.feat-card h3 { font-size: 18px; font-weight: 700; color: var(--el-text-color-primary); margin-bottom: 8px; }
.feat-card p { font-size: 15px; color: var(--el-text-color-regular); line-height: 1.6; }
@media (max-width: 1024px) { .features-grid { grid-template-columns: repeat(2, 1fr); } }
@media (max-width: 640px) { .features-grid { grid-template-columns: 1fr; } }
.gallery-grid {
 display: grid; grid-template-columns: repeat(4, 1fr); gap: 16px;
}
.gallery-item {
 border-radius: 20px; overflow: hidden;
 border: 1px solid var(--el-border-color-light);
 transition: transform 0.2s, box-shadow 0.2s;
 position: relative;
}
.gallery-item:hover {
 transform: translateY(-4px);
 box-shadow: 0 8px 24px rgba(0,0,0,0.1);
}
.gallery-item img {
 width: 100%; height: auto; display: block;
}
.gallery-caption {
 padding: 12px 14px; background: var(--el-bg-color);
}
.gallery-caption h4 {
 font-size: 13px; font-weight: 700; color: var(--el-text-color-primary);
 margin-bottom: 2px;
}
.gallery-caption p {
 font-size: 11px; color: var(--el-text-color-secondary); line-height: 1.4;
}
.gallery-note {
 text-align: center; margin-top: 20px;
 font-size: 13px; color: var(--el-text-color-secondary); font-style: italic;
}
@media (max-width: 1024px) { .gallery-grid { grid-template-columns: repeat(2, 1fr); } }
@media (max-width: 480px) { .gallery-grid { grid-template-columns: 1fr; } }
html.dark .gallery-item { border-color: var(--el-border-color); }
html.dark .gallery-caption { background: var(--el-bg-color-page); }
html.dark .gallery-caption h4 { color: var(--el-text-color-primary); }
html.dark .gallery-caption p { color: var(--el-text-color-regular); }
.code-split {
 display: flex; gap: 48px; align-items: flex-start;
}
.code-left { flex: 1; min-width: 0; }
.code-right { flex: 1; }
.code-wrap {
 border-radius: 16px !important; overflow: hidden !important;
 border: 1px solid #334155 !important; background: #0f172a !important;
}
.markdown-body .nb-page .code-wrap {
 border-radius: 16px !important; overflow: hidden !important;
 border: 1px solid #334155 !important; background: #0f172a !important;
}
.code-bar {
 display: flex !important; align-items: center !important; justify-content: space-between !important;
 padding: 12px 20px !important; background: #1e293b !important;
 border-bottom: 1px solid #334155 !important;
}
.code-dots { display: flex; gap: 6px; }
.code-dots i {
 width: 10px; height: 10px; border-radius: 50%;
 display: inline-block;
}
.code-dots .r { background: #ef4444; }
.code-dots .y { background: #f59e0b; }
.code-dots .g { background: #10b981; }
.code-lang {
 font-size: 12px; color: var(--el-text-color-secondary); font-weight: 600;
 text-transform: uppercase; letter-spacing: 0.05em;
}
.code-block {
 padding: 24px !important; margin: 0 !important; overflow-x: auto !important;
 font-family: 'JetBrains Mono', 'Fira Code', 'SF Mono', monospace !important;
 font-size: 13.5px !important; line-height: 1.7 !important; color: #e2e8f0 !important;
 white-space: pre !important; background: transparent !important;
 border: none !important; border-radius: 0 !important;
}
.markdown-body .nb-page .code-block {
 padding: 24px !important; margin: 0 !important; overflow-x: auto !important;
 font-family: 'JetBrains Mono', 'Fira Code', 'SF Mono', monospace !important;
 font-size: 13.5px !important; line-height: 1.7 !important; color: #e2e8f0 !important;
 white-space: pre !important; background: transparent !important;
 border: none !important; border-radius: 0 !important;
}
.code-right h2 {
 font-size: clamp(24px, 3vw, 32px);
 font-weight: 700; color: var(--el-text-color-primary); margin-bottom: 12px;
 letter-spacing: normal;
}
.code-right > p { font-size: 16px; color: var(--el-text-color-regular); line-height: 1.6; margin-bottom: 32px; }
.explain-steps { display: flex; flex-direction: column; gap: 20px; }
.explain-step { display: flex; gap: 16px; align-items: flex-start; }
.step-num {
 width: 32px; height: 32px; border-radius: 50%;
 background: var(--el-bg-color-page); border: 1px solid var(--el-border-color-light);
 display: flex; align-items: center; justify-content: center;
 font-size: 14px; font-weight: 700; color: var(--el-text-color-regular);
 flex-shrink: 0;
}
.step-text h4 { font-size: 15px; font-weight: 700; color: var(--el-text-color-primary); margin-bottom: 2px; }
.step-text p { font-size: 14px; color: var(--el-text-color-secondary); line-height: 1.5; }
@media (max-width: 768px) {
 .code-split { flex-direction: column; }
 .code-left { order: 2; }
 .code-right { order: 1; }
}
.actions-grid {
 display: grid; grid-template-columns: repeat(4, 1fr); gap: 20px;
}
.act-card {
 padding: 28px 24px; background: var(--el-bg-color);
 border: none; border-radius: 20px; box-shadow: 0 2px 12px 0 rgba(0,0,0,0.08);
 text-align: center;
 transition: border-color 0.2s, box-shadow 0.2s, transform 0.15s;
}
.act-card:hover { box-shadow: 0 8px 24px 0 rgba(0,0,0,0.12);
 transform: translateY(-2px);
}
.act-icon { font-size: 36px; margin-bottom: 16px; }
.act-card h3 { font-size: 17px; font-weight: 700; color: var(--el-text-color-primary); margin-bottom: 8px; }
.act-card p { font-size: 14px; color: var(--el-text-color-regular); line-height: 1.6; }
@media (max-width: 1024px) { .actions-grid { grid-template-columns: repeat(2, 1fr); } }
@media (max-width: 480px) { .actions-grid { grid-template-columns: 1fr; } }
.usecases-grid {
 display: grid; grid-template-columns: repeat(4, 1fr); gap: 20px;
}
.uc-card {
 padding: 28px 24px; background: var(--el-bg-color);
 border: none; border-radius: 20px; box-shadow: 0 2px 12px 0 rgba(0,0,0,0.08);
 text-align: center;
 transition: border-color 0.2s, box-shadow 0.2s, transform 0.15s;
}
.uc-card:hover { box-shadow: 0 8px 24px 0 rgba(0,0,0,0.12);
 transform: translateY(-2px);
}
.uc-icon { font-size: 36px; margin-bottom: 16px; }
.uc-card h3 { font-size: 17px; font-weight: 700; color: var(--el-text-color-primary); margin-bottom: 8px; }
.uc-card p { font-size: 14px; color: var(--el-text-color-regular); line-height: 1.6; }
@media (max-width: 1024px) { .usecases-grid { grid-template-columns: repeat(2, 1fr); } }
@media (max-width: 480px) { .usecases-grid { grid-template-columns: 1fr; } }
.steps-row {
 display: flex; align-items: flex-start; justify-content: center;
 margin-bottom: 48px;
}
.stp-card { flex: 1; max-width: 320px; text-align: center; padding: 0 24px; }
.stp-num {
 font-size: clamp(48px, 6vw, 72px);
 font-weight: 700; color: #e2e8f0;
 letter-spacing: -0.04em; line-height: 1;
 margin-bottom: 20px;
}
.stp-card h3 { font-size: 18px; font-weight: 700; color: var(--el-text-color-primary); margin-bottom: 10px; }
.stp-card p { font-size: 15px; color: var(--el-text-color-regular); line-height: 1.6; }
.stp-conn {
 width: 60px; height: 2px; background: var(--el-border-color-light);
 margin-top: 36px; flex-shrink: 0;
}
.steps-cta { text-align: center; }
@media (max-width: 768px) {
 .steps-row { flex-direction: column; align-items: center; gap: 32px; }
 .stp-conn { width: 2px; height: 32px; margin: 0; }
 .stp-card { max-width: 100%; }
}
.cmp-wrap { overflow-x: auto; -webkit-overflow-scrolling: touch; }
.nb-page .cmp-table {
 display: table !important;
 width: 100%; max-width: 860px; margin: 0 auto;
 border-collapse: collapse; font-size: 15px;
}
.nb-page .cmp-table th, .cmp-table td {
 padding: 16px 20px; text-align: center;
 border-bottom: 1px solid var(--el-border-color-light);
}
.nb-page .cmp-table th {
 font-weight: 700; color: var(--el-text-color-regular); font-size: 14px;
 text-transform: uppercase; letter-spacing: 0.04em;
 background: var(--el-bg-color-page);
}
.nb-page .cmp-table td:first-child, .cmp-table th:first-child {
 text-align: left; font-weight: 600; color: var(--el-text-color-primary);
}
.cmp-us { font-weight: 700; }
.cmp-brand { font-weight: 700; color: var(--el-text-color-primary); }
.ck { color: #10b981; font-weight: 700; font-size: 18px; }
.cx { color: #d1d5db; font-weight: 700; font-size: 18px; }
@media (max-width: 640px) {
 .cmp-table th, .cmp-table td { padding: 12px 10px; font-size: 13px; }
}
.models-grid {
 display: grid; grid-template-columns: repeat(2, 1fr);
 gap: 24px; max-width: 720px; margin: 0 auto;
}
.mdl-card {
 padding: 32px 28px;
 border: none; border-radius: 20px; box-shadow: 0 2px 12px 0 rgba(0,0,0,0.08);
 background: var(--el-bg-color); position: relative;
}
.mdl-card.mdl-rec { border-color: #4285F4; border-width: 2px; }
.mdl-rec-badge {
 position: absolute; top: -12px; left: 50%;
 transform: translateX(-50%);
 padding: 4px 14px; background: #4285F4; color: #ffffff;
 border-radius: 9999px; font-size: 12px; font-weight: 700;
 text-transform: uppercase; letter-spacing: 0.04em;
}
.mdl-head { display: flex; align-items: center; gap: 10px; margin-bottom: 12px; }
.mdl-head h3 { font-size: 20px; font-weight: 700; color: var(--el-text-color-primary); }
.mdl-tag {
 padding: 3px 10px; background: var(--el-bg-color-page); border-radius: 9999px;
 font-size: 11px; font-weight: 700; color: var(--el-text-color-regular);
 text-transform: uppercase; letter-spacing: 0.04em;
}
.mdl-tag-blue { background: #eff6ff; color: #2563eb; }
.mdl-tag-purple { background: #EBF2FE; color: #4285F4; }
.nb-page .mdl-desc { font-size: 15px; color: var(--el-text-color-regular); line-height: 1.6; margin-bottom: 20px; }
.mdl-feats { display: flex; flex-direction: column; gap: 8px; }
.mdl-feats li { font-size: 14px; color: var(--el-text-color-regular); line-height: 1.4; }
@media (max-width: 768px) { .models-grid { grid-template-columns: 1fr; } }
.price-grid {
 display: grid !important; grid-template-columns: repeat(2, 1fr) !important;
 gap: 24px !important; max-width: 720px !important; margin: 0 auto !important;
 align-items: start;
}
.price-card {
 padding: 36px 32px;
 border: 1px solid var(--el-border-color-light); border-radius: 20px;
 background: var(--el-bg-color); position: relative;
}
.price-card-feat {
 border: 2px solid #4285F4;
 box-shadow: 0 8px 32px rgba(0,0,0,0.08);
 transform: scale(1.03);
}
.price-feat-badge {
 position: absolute; top: -13px; left: 50%;
 transform: translateX(-50%);
 padding: 5px 18px; background: #4285F4; color: #ffffff;
 border-radius: 9999px; font-size: 12px; font-weight: 700;
 text-transform: uppercase; letter-spacing: 0.04em;
 white-space: nowrap;
}
.price-tier {
 font-size: 16px; font-weight: 700; color: var(--el-text-color-regular);
 text-transform: uppercase; letter-spacing: 0.06em; margin-bottom: 12px;
}
.price-amt {
 font-size: clamp(36px, 5vw, 48px);
 font-weight: 700; color: var(--el-text-color-primary); letter-spacing: normal;
}
.price-per { font-size: 16px; color: var(--el-text-color-secondary); font-weight: 500; }
.nb-page .price-desc { font-size: 14px; color: var(--el-text-color-secondary); margin-bottom: 24px; margin-top: 8px; }
.nb-page .price-feats { display: flex; flex-direction: column; gap: 10px; margin-bottom: 36px; }
.nb-page .price-feats li { font-size: 14px; color: var(--el-text-color-regular); line-height: 1.4; display: flex; align-items: center; gap: 8px; }
.price-ck { color: #10b981; font-weight: 700; font-size: 14px; flex-shrink: 0; }
.price-btn {
 display: block; text-align: center; padding: 14px 0;
 border-radius: 9999px; font-size: 15px; font-weight: 600;
 transition: background 0.2s, border-color 0.2s, transform 0.15s;
 width: 100%; cursor: pointer;
}
.nb-page .price-btn-fill { background: #4285F4; color: #ffffff !important; border: none; text-decoration: none !important; }
.nb-page .price-btn-fill:hover { background: #3367D6; transform: translateY(-1px); text-decoration: none !important; }
.nb-page .price-btn-out { background: var(--el-bg-color); color: var(--el-text-color-primary) !important; border: 1px solid var(--el-border-color-light); text-decoration: none !important; }
.nb-page .price-btn-out:hover { background: var(--el-bg-color-page); text-decoration: none !important; }
@media (max-width: 768px) {
 .price-grid { grid-template-columns: minmax(0,1fr) !important; }
 .price-card-feat { transform: none; }
}
.faq-list { display: flex; flex-direction: column; }
.faq-item { border-bottom: 1px solid var(--el-border-color-light); }
.faq-item:first-child { border-top: 1px solid #e5e7eb; }
.faq-q {
 display: flex; justify-content: space-between; align-items: center;
 padding: 20px 0; cursor: pointer;
 font-size: 16px; font-weight: 600; color: var(--el-text-color-primary);
 list-style: none; user-select: none;
 transition: color 0.2s;
}
.faq-q::-webkit-details-marker { display: none; }
.faq-q:hover { color: var(--el-text-color-primary); }
.faq-chev { font-size: 18px; color: var(--el-text-color-secondary); transition: transform 0.2s; flex-shrink: 0; }
.faq-item[open] .faq-chev { transform: rotate(180deg); }
.faq-a { padding: 0 0 20px; }
.faq-a p { font-size: 15px; color: var(--el-text-color-regular); line-height: 1.7; }
.rel-grid {
 display: grid; grid-template-columns: repeat(2, 1fr);
 gap: 16px; max-width: 800px; margin: 0 auto;
}
.rel-card {
 display: flex; align-items: center; gap: 16px;
 padding: 20px 24px; background: var(--el-bg-color);
 border: none; border-radius: 20px; box-shadow: 0 2px 12px 0 rgba(0,0,0,0.08);
 transition: border-color 0.2s, box-shadow 0.2s;
}
.rel-card:hover { box-shadow: 0 4px 12px rgba(0,0,0,0.05); }
.rel-icon { font-size: 28px; flex-shrink: 0; }
.rel-info { flex: 1; min-width: 0; }
.rel-info h3 { font-size: 15px; font-weight: 700; color: var(--el-text-color-primary); margin-bottom: 2px; }
.rel-info p { font-size: 13px; color: var(--el-text-color-secondary); line-height: 1.4; }
.rel-arrow {
 font-size: 18px; color: #cbd5e1; flex-shrink: 0;
 transition: color 0.2s, transform 0.2s;
}
.rel-card:hover .rel-arrow { color: var(--el-text-color-regular); transform: translateX(3px); }
@media (max-width: 640px) { .rel-grid { grid-template-columns: 1fr; } }
.nb-cta {
 padding: 100px 0; background: #0f172a;
 text-align: center; position: relative; overflow: hidden;
}
.nb-cta::before {
 content: '';
 position: absolute; top: -100px; left: 50%;
 transform: translateX(-50%);
 width: 700px; height: 400px;
 background: radial-gradient(ellipse, rgba(66, 133, 244, 0.12) 0%, transparent 70%);
 pointer-events: none;
}
.nb-cta h2 {
 font-size: clamp(28px, 4vw, 44px);
 font-weight: 700; color: #f8fafc;
 letter-spacing: normal; margin-bottom: 28px;
 position: relative;
}
.nb-cta > div > p {
 font-size: clamp(16px, 2vw, 18px);
 color: var(--el-text-color-secondary); max-width: 520px;
 margin: 0 auto 56px; line-height: 1.6;
 position: relative;
}
.cta-actions {
 display: flex; gap: 12px; justify-content: center;
 flex-wrap: wrap; position: relative;
}
.nb-page .btn-cta-light {
 display: inline-flex; align-items: center; gap: 6px;
 padding: 14px 32px; background: #4285F4; color: #ffffff !important;
 border-radius: 9999px; font-size: 15px; font-weight: 700;
 transition: background 0.2s, transform 0.15s;
 text-decoration: none !important;
}
.nb-page .btn-cta-light:hover { background: #3367D6; transform: translateY(-1px); text-decoration: none !important; }
.nb-page .btn-cta-ghost {
 display: inline-flex; align-items: center;
 padding: 14px 32px; background: transparent; color: #94a3b8 !important;
 border: 1px solid #334155; border-radius: 9999px;
 font-size: 15px; font-weight: 600;
 transition: border-color 0.2s, color 0.2s;
 text-decoration: none !important;
}
.nb-page .btn-cta-ghost:hover { border-color: var(--el-text-color-regular); color: #e2e8f0 !important; text-decoration: none !important; }
.nb-page code {
 background: #dbeafe !important;
 padding: 2px 8px !important;
 border-radius: 5px !important;
 font-size: 13px !important;
 font-family: 'JetBrains Mono', 'Fira Code', 'SF Mono', monospace !important;
 color: #1e40af !important;
 border: 1px solid #bfdbfe !important;
}
.s-text-dark { color: var(--el-text-color-primary); }
.s-text-brand { color: #4285F4; }
.s-section-body { font-size: 16px; color: var(--el-text-color-regular); line-height: 1.8; text-align: center; max-width: 680px; margin: 0 auto; }
.s-section-body p + p { margin-top: 16px; }
.s-text-muted { color: var(--el-text-color-secondary); }
.tag-row {
 display: flex; gap: 8px; flex-wrap: wrap;
 justify-content: center; margin-top: 16px;
}
.tag-item {
 padding: 4px 12px; background: var(--el-bg-color-page);
 border: 1px solid var(--el-border-color-light); border-radius: 9999px;
 font-size: 12px; font-weight: 600; color: var(--el-text-color-regular);
}
html.dark .nb-page { background: var(--el-bg-color); color: var(--el-text-color-primary); }
html.dark .nb-page a { color: inherit; }
html.dark .markdown-body .nb-page a { color: inherit !important; }
html.dark .markdown-body .nb-page a.s-btn-primary,
html.dark .markdown-body .nb-page a.price-btn-fill,
html.dark .markdown-body .nb-page a.btn-cta-light { color: #ffffff !important; }
html.dark .markdown-body .nb-page a.s-btn-secondary { color: var(--el-text-color-primary) !important; }
html.dark .markdown-body .nb-page a.price-btn-out { color: var(--el-text-color-primary) !important; }
html.dark .markdown-body .nb-page a.btn-cta-ghost { color: #94a3b8 !important; }
html.dark .markdown-body .nb-page a.btn-cta-ghost:hover { color: var(--el-text-color-primary) !important; }
html.dark .s-bg-white { background: var(--el-bg-color); }
html.dark .s-bg-gray { background: var(--el-bg-color-page); }
html.dark .s-bg-dark { background: var(--el-bg-color); }
html.dark .s-header h2 { color: var(--el-text-color-primary); }
html.dark .s-header p { color: var(--el-text-color-secondary); }
html.dark .nb-page .s-btn-primary { background: #4285F4; color: #ffffff !important; }
html.dark .nb-page .s-btn-primary:hover { background: #3367D6; }
html.dark .nb-page .s-btn-secondary {
 background: #1e293b; color: var(--el-text-color-primary) !important;
 border-color: #475569;
}
html.dark .nb-page .s-btn-secondary:hover { background: var(--el-border-color); border-color: var(--el-text-color-regular); }
html.dark .nb-hero { background: var(--el-bg-color); }
html.dark .nb-hero::before {
 background: radial-gradient(ellipse, rgba(66, 133, 244, 0.15) 0%, transparent 70%);
}
html.dark .hero-badge { background: var(--el-bg-color-page); border-color: var(--el-border-color); color: var(--el-text-color-secondary); }
html.dark .nb-hero h1 { color: var(--el-text-color-primary); }
html.dark .nb-hero h1 span { color: #6EA8FE; }
html.dark .nb-page .hero-subtitle { color: var(--el-text-color-secondary); }
html.dark .hero-highlights .h-item { color: var(--el-text-color-secondary); }
html.dark .hero-highlights .h-div { background: var(--el-border-color); }
html.dark .nb-stats { background: var(--el-bg-color-page); border-color: var(--el-border-color); }
html.dark .stat-val { color: var(--el-text-color-primary); }
html.dark .stat-lbl { color: var(--el-text-color-regular); }
html.dark .feat-card {
 background: var(--el-bg-color-page); border-color: var(--el-border-color);
}
html.dark .feat-card:hover { border-color: var(--el-text-color-regular); box-shadow: 0 4px 16px rgba(0,0,0,0.3); }
html.dark .feat-card h3 { color: var(--el-text-color-primary); }
html.dark .feat-card p { color: var(--el-text-color-secondary); }
html.dark .code-right h2 { color: var(--el-text-color-primary); }
html.dark .code-right > p { color: var(--el-text-color-secondary); }
html.dark .step-num { background: var(--el-border-color); border-color: var(--el-text-color-regular); color: var(--el-text-color-secondary); }
html.dark .step-text h4 { color: var(--el-text-color-primary); }
html.dark .step-text p { color: var(--el-text-color-regular); }
html.dark .nb-page code {
 background: #1e3a5f !important; color: #93c5fd !important; border-color: #2563eb !important;
}
html.dark .s-text-dark { color: var(--el-text-color-primary); }
html.dark .s-text-brand { color: #6EA8FE; }
html.dark .s-section-body { color: var(--el-text-color-secondary); }
html.dark .act-card { background: var(--el-bg-color-page); border-color: var(--el-border-color); }
html.dark .act-card:hover { border-color: var(--el-text-color-regular); box-shadow: 0 4px 16px rgba(0,0,0,0.3); }
html.dark .act-card h3 { color: var(--el-text-color-primary); }
html.dark .act-card p { color: var(--el-text-color-secondary); }
html.dark .uc-card { background: var(--el-bg-color-page); border-color: var(--el-border-color); }
html.dark .uc-card:hover { border-color: var(--el-text-color-regular); box-shadow: 0 4px 16px rgba(0,0,0,0.3); }
html.dark .uc-card h3 { color: var(--el-text-color-primary); }
html.dark .uc-card p { color: var(--el-text-color-secondary); }
html.dark .stp-num { color: #334155; }
html.dark .stp-card h3 { color: var(--el-text-color-primary); }
html.dark .stp-card p { color: var(--el-text-color-secondary); }
html.dark .stp-conn { background: var(--el-border-color); }
html.dark .cmp-table th { background: var(--el-bg-color-page); color: var(--el-text-color-secondary); }
html.dark .cmp-table td { border-color: var(--el-border-color); }
html.dark .cmp-table th { border-color: var(--el-border-color); }
html.dark .cmp-table td:first-child { color: var(--el-text-color-primary); }
html.dark .cmp-brand { color: var(--el-text-color-primary); }
html.dark .cx { color: var(--el-text-color-regular); }
html.dark .mdl-card { background: var(--el-bg-color-page); border-color: var(--el-border-color); }
html.dark .mdl-card.mdl-rec { border-color: #4285F4; }
html.dark .mdl-head h3 { color: var(--el-text-color-primary); }
html.dark .mdl-tag { background: var(--el-border-color); color: var(--el-text-color-secondary); }
html.dark .mdl-tag-blue { background: #1e3a5f; color: #60a5fa; }
html.dark .mdl-tag-purple { background: rgba(66, 133, 244, 0.2); color: #6EA8FE; }
html.dark .mdl-desc { color: var(--el-text-color-secondary); }
html.dark .mdl-feats li { color: var(--el-text-color-secondary); }
html.dark .price-card { background: var(--el-bg-color-page); border-color: var(--el-border-color); }
html.dark .price-card-feat { border-color: #4285F4; box-shadow: 0 8px 32px rgba(0,0,0,0.3); }
html.dark .price-tier { color: var(--el-text-color-secondary); }
html.dark .price-amt { color: var(--el-text-color-primary); }
html.dark .price-desc { color: var(--el-text-color-regular); }
html.dark .price-feats li { color: var(--el-text-color-secondary); }
html.dark .nb-page .price-btn-out {
 background: #1e293b; color: var(--el-text-color-primary) !important; border-color: #334155;
}
html.dark .nb-page .price-btn-out:hover { background: var(--el-border-color); border-color: var(--el-text-color-regular); }
html.dark .faq-item { border-color: var(--el-border-color); }
html.dark .faq-q { color: var(--el-text-color-primary); }
html.dark .faq-q:hover { color: #ffffff; }
html.dark .faq-chev { color: var(--el-text-color-regular); }
html.dark .faq-a p { color: var(--el-text-color-secondary); }
html.dark .rel-card { background: var(--el-bg-color-page); border-color: var(--el-border-color); }
html.dark .rel-card:hover { border-color: var(--el-text-color-regular); box-shadow: 0 4px 12px rgba(0,0,0,0.3); }
html.dark .rel-info h3 { color: var(--el-text-color-primary); }
html.dark .rel-info p { color: var(--el-text-color-regular); }
html.dark .rel-arrow { color: var(--el-text-color-regular); }
html.dark .rel-card:hover .rel-arrow { color: var(--el-text-color-secondary); }
html.dark .nb-cta { background: #020617; }
html.dark .nb-cta::before {
 background: radial-gradient(ellipse, rgba(66, 133, 244, 0.2) 0%, transparent 70%);
}
html.dark .tag-item { background: var(--el-border-color); border-color: var(--el-text-color-regular); color: var(--el-text-color-secondary); }
html.dark .nb-page .btn-cta-light { color: #ffffff !important; }
html.dark .nb-page .btn-cta-ghost { color: #94a3b8 !important; }
html.dark .nb-page .btn-cta-ghost:hover { color: var(--el-text-color-primary) !important; }
html.dark .nb-page .price-btn-fill { color: #ffffff !important; }
.nb-page .code-left,.nb-page .code-right{width:100%;max-width:100%;min-width:0}
.nb-page .code-wrap{max-width:100%;min-width:0}
</style><div class="nb-page"><section class="nb-hero">
 <div class="s-container-narrow">
 <div class="hero-badge">
 <span class="badge-dot"></span>
 Nano Banana API · Ace Data Cloud
 </div>
 <h1>
 Nano Banana API：<br/>
 Generate <span>AI Images</span>
 </h1>
 <p class="hero-subtitle">
 Powered by Google Gemini 2.5 Flash/3 Pro Image models, enabling high-quality image generation and editing through a simple REST API. Supports multiple scenarios including text-to-image, multi-image editing, virtual try-on, and product background replacement.
 </p>
 <div class="hero-actions">
 <a href="https://platform.acedata.cloud/documents/nano-banana-images" class="s-btn-primary">📄 View Documentation</a>
 </div>
 <div class="hero-highlights">
 <span class="h-item">🖼️ 2 Operation Modes</span>
 <span class="h-div"></span>
 <span class="h-item">🤖 2 Model Versions</span>
 <span class="h-div"></span>
 <span class="h-item">📐 7 Aspect Ratios</span>
 <span class="h-div"></span>
 <span class="h-item">🔑 Bearer Token Authentication</span>
 </div>
 </div>
</section>
<section class="nb-stats s-section-sm s-bg-gray">
 <div class="s-container">
 <div class="stats-grid">
 <div>
 <div class="stat-icon">🖼️</div>
 <div class="stat-val">2</div>
 <div class="stat-lbl">Operation Modes</div>
 </div>
 <div>
 <div class="stat-icon">🤖</div>
 <div class="stat-val">2</div>
 <div class="stat-lbl">Model Versions</div>
 </div>
 <div>
 <div class="stat-icon">📡</div>
 <div class="stat-val">2</div>
 <div class="stat-lbl">API Endpoints</div>
 </div>
 <div>
 <div class="stat-icon">📐</div>
 <div class="stat-val">7</div>
 <div class="stat-lbl">Aspect Ratio Options</div>
 </div>
 </div>
 </div>
</section>
<section class="s-section s-bg-white">
 <div class="s-container-narrow">
 <div class="s-header">
 <h2>What Is Nano Banana?</h2>
 </div>
 <div class="s-section-body">
 <p><strong class="s-text-brand">Nano Banana</strong> is a unified API wrapper based on Google Gemini image generation models. It simplifies and optimizes the Gemini 2.5 Flash Image and Gemini 3 Pro Image models, providing a more user-friendly interface and lower pricing.</p>
 <p>Ace Data Cloud offers<strong class="s-text-dark">lower prices than the official service</strong> (approximately 1/3 of the official price), along with<strong class="s-text-brand">higher concurrency support</strong>, dedicated customer service, and 24/7 stability assurance. No need to handle complex Google Cloud configurations—ready to use out of the box.</p>
 </div>
 </div>
</section><section class="s-section s-bg-gray">
 <div class="s-container">
 <div class="s-header">
 <h2>Core Capabilities of the Nano Banana API</h2>
 <p>Text-to-image generation and multi-image editing, covering the complete image creation workflow</p>
 </div>
 <div class="features-grid">
 <div class="feat-card">
 <div class="feat-icon">✨</div>
 <h3>High-Quality Text-to-Image Generation</h3>
 <p>Enter detailed text descriptions (subject, mood, lighting, camera) to generate professional-grade, high-quality images. Suitable for brand visuals, product posters, cover images, and more.</p>
 </div>
 <div class="feat-card">
 <div class="feat-icon">🔀</div>
 <h3>Multi-Image Combined Editing</h3>
 <p>Upload multiple images (such as a portrait + clothing), and AI will intelligently blend them. Supports advanced editing operations such as virtual try-on, product placement, and scene compositing.</p>
 </div>
 <div class="feat-card">
 <div class="feat-icon">👗</div>
 <h3>Virtual Outfit Change</h3>
 <p>Provide a portrait photo and a clothing PNG to automatically create a dressed-up result. Ideal for e-commerce apparel displays and quickly expanding livestream image content.</p>
 </div>
 <div class="feat-card">
 <div class="feat-icon">🏠</div>
 <h3>Product Background Replacement</h3>
 <p>Place white-background product images into real scenes (wooden tables, grass, bathrooms, desks) to make product detail pages richer and more lifelike.</p>
 </div>
 <div class="feat-card">
 <div class="feat-icon">🎨</div>
 <h3>Attribute Replacement</h3>
 <p>Change materials, colors, and styles. Swap a bag to leather, a drink to another flavor, or shoes to a different colorway—making visual SKU experimentation easier.</p>
 </div>
 <div class="feat-card">
 <div class="feat-icon">⚡</div>
 <h3>Asynchronous Webhook</h3>
 <p>Set <code>callback_url</code>, and results will be automatically pushed after the task is completed. No polling required, ideal for batch production scenarios.</p>
 </div>
 </div>
 </div>
</section>
<section class="s-section s-bg-white">
 <div class="s-container">
 <div class="s-header">
 <h2>AI-Generated Work Showcase</h2>
 <p>The images below were actually generated by the Nano Banana API—what you see is what you get</p>
 </div>
 <div class="gallery-grid">
 <div class="gallery-item">
 <img src="https://cdn.acedata.cloud/d635720766.png" alt="White porcelain coffee cup on a windowsill in morning light" loading="lazy">
 <div class="gallery-caption">
 <h4>Morning Coffee Cup</h4>
 <p>nano-banana · 3:2 · Text-to-image</p>
 </div>
 </div>
 <div class="gallery-item">
 <img src="https://cdn.acedata.cloud/87f62c94a4.png" alt="Cyberpunk city skyline" loading="lazy">
 <div class="gallery-caption">
 <h4>Cyber City Skyline</h4>
 <p>nano-banana · 16:9 · Text-to-image</p>
 </div>
 </div>
 <div class="gallery-item">
 <img src="https://cdn.acedata.cloud/3d1ed0dc1f.png" alt="Luxury perfume product photography" loading="lazy">
 <div class="gallery-caption">
 <h4>Luxury Product Photography</h4>
 <p>nano-banana-pro · 1:1 · Text-to-image</p>
 </div>
 </div>
 <div class="gallery-item">
 <img src="https://cdn.acedata.cloud/8b86d640af.png" alt="Golden retriever puppy with sunflowers" loading="lazy">
 <div class="gallery-caption">
 <h4>Golden Retriever Puppy in the Sun</h4>
 <p>nano-banana · 3:4 · Text-to-image</p>
 </div>
 </div>
 </div>
 <p class="gallery-note">💡 All images were generated in a single API call, without any post-processing</p>
 </div>
</section><section class="s-section s-bg-white">
 <div class="s-container">
 <div class="code-split">
 <div class="code-left">
 <div class="code-wrap">
 <div class="code-bar">
 <div class="code-dots"><i class="r"></i><i class="y"></i><i class="g"></i></div>
 <div class="code-lang">cURL</div>
 </div>
 <pre class="code-block">curl -X POST https://api.acedata.cloud/nano-banana/images \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "action": "generate",
    "prompt": "白瓷咖啡杯，晨光窗台，85mm镜头，浅景深，柔和高光，治愈干净",
    "model": "nano-banana",
    "aspect_ratio": "3:2"
  }'</pre>
 </div>
 <div style="margin-top: 16px;">
 <div class="code-wrap">
 <div class="code-bar">
 <div class="code-dots"><i class="r"></i><i class="y"></i><i class="g"></i></div>
 <div class="code-lang">Response</div>
 </div>
 <pre class="code-block">{
  "success": true,
  "task_id": "c1075552-a527-4a70-8d98-ef783f4087c1",
  "trace_id": "3352b744-d17e-4d01-b1ef-a8c8e2ca3d2e",
  "data": [{
    "image_url": "https://cdn.acedata.cloud/d635720766.png"
  }]
}</pre>
 </div>
 </div>
 </div>
 <div class="code-right">
 <h2>Quick Start—Get Started in 3 Minutes</h2>
 <p>A simple REST API with Bearer Token authentication. Generate your first AI image with a single request.</p>
 <div class="explain-steps">
 <div class="explain-step">
 <div class="step-num">1</div>
 <div class="step-text">
 <h4>Get an API Key</h4>
 <p>Register with Ace Data Cloud and get your Bearer Token from the console</p>
 </div>
 </div>
 <div class="explain-step">
 <div class="step-num">2</div>
 <div class="step-text">
 <h4>Send a POST Request</h4>
 <p>Send a request to <code>/nano-banana/images</code> with a prompt and parameters</p>
 </div>
 </div>
 <div class="explain-step">
 <div class="step-num">3</div>
 <div class="step-text">
 <h4>Get the Image URL</h4>
 <p>Receive a permanently accessible image URL—ready for production use immediately</p>
 </div>
 </div>
 </div>
 </div>
 </div>
 </div>
</section>
<section class="s-section s-bg-gray">
 <div class="s-container">
 <div class="s-header">
 <h2>Use Cases</h2>
 <p>From e-commerce content to brand creativity—Nano Banana covers these scenarios</p>
 </div>
 <div class="usecases-grid">
 <div class="uc-card">
 <div class="uc-icon">👗</div>
 <h3>E-commerce Apparel</h3>
 <p>Have an influencer take a single styled photo, then use different clothing PNGs to batch-generate outfit images and quickly expand your store assets</p>
 </div>
 <div class="uc-card">
 <div class="uc-icon">📦</div>
 <h3>Product Detail Pages</h3>
 <p>Use a single product image on a white background to compose images in multiple settings such as wooden tables, grass, and bathrooms, making detail pages richer and more convincing</p>
 </div>
 <div class="uc-card">
 <div class="uc-icon">🎨</div>
 <h3>Brand Visuals</h3>
 <p>Quickly generate brand key visuals, campaign posters, and cover images. Switch the same key visual between styles and holiday themes with one click</p>
 </div>
 <div class="uc-card">
 <div class="uc-icon">🤖</div>
 <h3>AI Agent Integration</h3>
 <p>Integrate with Claude and ChatGPT through an MCP Server or Dify plugin to enable natural-language image generation</p>
 </div>
 </div>
 </div>
</section><section class="s-section s-bg-white">
 <div class="s-container">
 <div class="s-header">
 <h2>Advanced Features</h2>
 <p>Nano Banana is more than simple text-to-image generation—it can also handle these advanced tasks</p>
 </div>
 <div class="actions-grid">
 <div class="act-card">
 <div class="act-icon">🎭</div>
 <h3>2D to 3D Figurines</h3>
 <p>Convert anime characters/portraits into commercialized figurine models, complete with packaging box displays</p>
 </div>
 <div class="act-card">
 <div class="act-icon">🔧</div>
 <h3>Product Exploded Views</h3>
 <p>Showcase a product's internal structure, with metal parts and electronic components separated and suspended for a technical aesthetic</p>
 </div>
 <div class="act-card">
 <div class="act-icon">📷</div>
 <h3>Old Photo Restoration</h3>
 <p>Restore scratched and damaged old black-and-white photos, enhance clarity, and colorize them naturally</p>
 </div>
 <div class="act-card">
 <div class="act-icon">🚗</div>
 <h3>Multi-Element Composites</h3>
 <p>Naturally blend multiple assets such as models, products, and backgrounds into a single high-quality image</p>
 </div>
 </div>
 <div class="tag-row" style="margin-top: 24px;">
 <span class="tag-item">+ Multi-angle shots</span>
 <span class="tag-item">+ Meme generation</span>
 <span class="tag-item">+ Sketch to photorealistic image</span>
 <span class="tag-item">+ Map to real-world scene</span>
 </div>
 </div>
</section>
<section class="s-section s-bg-gray">
 <div class="s-container">
 <div class="s-header">
 <h2>Get Started in 3 Quick Steps</h2>
 <p>From registration to generating your first AI image, it takes less than 3 minutes</p>
 </div>
 <div class="steps-row">
 <div class="stp-card">
 <div class="stp-num">01</div>
 <h3>Register and Get an API Key</h3>
 <p>Create a free account on Ace Data Cloud. Generate your Bearer Token from the API management console.</p>
 </div>
 <div class="stp-conn"></div>
 <div class="stp-card">
 <div class="stp-num">02</div>
 <h3>Make Your First API Call</h3>
 <p>Send a POST request with a text prompt to <code>/nano-banana/images</code>. You can use an SDK, cURL, or any HTTP client.</p>
 </div>
 <div class="stp-conn"></div>
 <div class="stp-card">
 <div class="stp-num">03</div>
 <h3>Integrate and Scale</h3>
 <p>Embed the API into your application. Use Webhooks for asynchronous processing and scale confidently to production.</p>
 </div>
 </div>
 <div class="steps-cta">
 <a href="https://platform.acedata.cloud/documents/nano-banana-images" class="s-btn-primary">View Documentation →</a>
 </div>
 </div>
</section><section class="s-section s-bg-white">
 <div class="s-container">
 <div class="s-header">
 <h2>Why Choose Ace Data Cloud?</h2>
 <p>Compare with Google Official and see our advantages</p>
 </div>
 <div class="cmp-wrap">
 <table class="cmp-table">
 <thead>
 <tr>
 <th>Feature</th>
 <th class="cmp-us"><span class="cmp-brand">Ace Data Cloud</span></th>
 <th>Google Official</th>
 </tr>
 </thead>
 <tbody>
 <tr>
 <td>Price</td>
 <td class="cmp-us"><strong>As low as $0.0133 / request</strong></td>
 <td>$0.039 Interactive / $0.02 Batch</td>
 </tr>
 <tr>
 <td>Setup Requirements</td>
 <td class="cmp-us"><span class="ck">✓</span> Ready to use instantly</td>
 <td><span class="cx">✗</span> Google Cloud configuration required</td>
 </tr>
 <tr>
 <td>Concurrency Support</td>
 <td class="cmp-us"><span class="ck">✓</span> High-concurrency guarantee</td>
 <td><span class="cx">✗</span> Low default quota</td>
 </tr>
 <tr>
 <td>Webhook Callbacks</td>
 <td class="cmp-us"><span class="ck">✓</span></td>
 <td>Partially supported</td>
 </tr>
 <tr>
 <td>Task Polling</td>
 <td class="cmp-us"><span class="ck">✓</span> Free</td>
 <td>—</td>
 </tr>
 <tr>
 <td>MCP Server</td>
 <td class="cmp-us"><span class="ck">✓</span></td>
 <td><span class="cx">✗</span></td>
 </tr>
 <tr>
 <td>Dify Plugin</td>
 <td class="cmp-us"><span class="ck">✓</span></td>
 <td><span class="cx">✗</span></td>
 </tr>
 <tr>
 <td>Dedicated Customer Support</td>
 <td class="cmp-us"><span class="ck">✓</span></td>
 <td><span class="cx">✗</span></td>
 </tr>
 <tr>
 <td>24/7 Monitoring</td>
 <td class="cmp-us"><span class="ck">✓</span></td>
 <td>Partially supported</td>
 </tr>
 </tbody>
 </table>
 </div>
 </div>
</section><section class="s-section s-bg-gray">
 <div class="s-container">
 <div class="s-header">
 <h2>Which model is right for you?</h2>
 <p>Choose the right model based on your quality and speed needs</p>
 </div>
 <div class="models-grid">
 <div class="mdl-card mdl-rec">
 <div class="mdl-rec-badge">Recommended</div>
 <div class="mdl-head">
 <h3>nano-banana</h3>
 <span class="mdl-tag-blue mdl-tag">Fast</span>
 </div>
 <p class="mdl-desc">Based on Gemini 2.5 Flash Image. Faster generation speeds and lower costs, ideal for batch content production and prototype validation.</p>
 <ul class="mdl-feats">
 <li>✓ Faster response times</li>
 <li>✓ As low as $0.0133 / call</li>
 <li>✓ 7 aspect ratios</li>
 <li>✓ Ideal for high-frequency scenarios</li>
 </ul>
 </div>
 <div class="mdl-card">
 <div class="mdl-head">
 <h3>nano-banana-2-lite</h3>
 <span class="mdl-tag-green mdl-tag">Lightweight</span>
 </div>
 <p class="mdl-desc">Based on Gemini 3.1 Flash Lite Image. Supports 1K resolution only, with fast image generation in 3-5 seconds.</p>
 <ul class="mdl-feats">
 <li>✓ Gemini 3.1 lightweight model</li>
 <li>✓ As low as $0.0133 / call</li>
 <li>✓ Supports 1K resolution only</li>
 <li>✓ Ideal for rapid validation</li>
 </ul>
 </div>
 <div class="mdl-card mdl-rec">
 <div class="mdl-rec-badge">New</div>
 <div class="mdl-head">
 <h3>nano-banana-2</h3>
 <span class="mdl-tag-green mdl-tag">Balanced</span>
 </div>
 <p class="mdl-desc">Based on Gemini 3.1 Flash Image. Pro-level quality + Flash speed, a great value choice.</p>
 <ul class="mdl-feats">
 <li>✓ Pro-level image quality</li>
 <li>✓ Flash-level response speed</li>
 <li>✓ As low as $0.0267 / call</li>
 <li>✓ Ideal for most scenarios</li>
 </ul>
 </div>
 <div class="mdl-card">
 <div class="mdl-head">
 <h3>nano-banana-pro</h3>
 <span class="mdl-tag-purple mdl-tag">High Quality</span>
 </div>
 <p class="mdl-desc">Based on Gemini 3 Pro Image. Highest-quality output with support for 2K/4K resolution. Ideal for flagship products and demanding scenarios.</p>
 <ul class="mdl-feats">
 <li>✓ Highest image quality</li>
 <li>✓ As low as $0.0333 / call</li>
 <li>✓ Supports 1K/2K/4K resolution</li>
 <li>✓ Ideal for brand visuals</li>
 </ul>
 </div>
 </div>
 </div>
</section><section class="s-section s-bg-white">
 <div class="s-container">
 <div class="s-header">
 <h2>Nano Banana API Pricing</h2>
 <p>Transparent pay-as-you-go pricing. No subscription fees. No hidden costs. Pay only for what you use.</p>
 </div>
 <div class="price-grid">
 <div class="price-card price-card-feat">
 <div class="price-feat-badge">Pay as you go</div>
 <div class="price-tier">Standard</div>
 <div>
 <span class="price-amt">$0.0133</span>
 <span class="price-per"> / call</span>
 </div>
 <p class="price-desc">nano-banana model (Gemini 2.5 Flash Image)<br>Save up to 27% with volume packages</p>
 <ul class="price-feats">
 <li><span class="price-ck">✓</span> Text-to-image (Generate)</li>
 <li><span class="price-ck">✓</span> Multi-image editing (Edit)</li>
 <li><span class="price-ck">✓</span> 7 aspect ratios</li>
 <li><span class="price-ck">✓</span> Webhook callbacks</li>
 <li><span class="price-ck">✓</span> Task polling—<strong>Free</strong></li>
 <li><span class="price-ck">✓</span> nano-banana-2-lite: as low as $0.0133 / call</li>
 <li><span class="price-ck">✓</span> nano-banana-2: as low as $0.0267 / call</li>
 <li><span class="price-ck">✓</span> nano-banana-pro: as low as $0.0333 / call</li>
 </ul>
 <a href="https://platform.acedata.cloud/services/nano-banana?tab=pricing" class="price-btn price-btn-fill">View pricing details</a>
 <a href="https://platform.acedata.cloud/documents/nano-banana-images" class="price-btn price-btn-out" style="margin-top:8px">View API documentation</a>
 </div>
 <div class="price-card">
 <div class="price-tier">Enterprise</div>
 <div>
 <span class="price-amt">Custom</span>
 </div>
 <p class="price-desc">Volume discounts for high-usage teams</p>
 <ul class="price-feats">
 <li><span class="price-ck">✓</span> Usage-based discounts</li>
 <li><span class="price-ck">✓</span> Priority support</li>
 <li><span class="price-ck">✓</span> Dedicated account manager</li>
 <li><span class="price-ck">✓</span> Custom rate limits</li>
 <li><span class="price-ck">✓</span> SLA guarantee</li>
 </ul>
 <a href="https://platform.acedata.cloud/support" class="price-btn price-btn-out">Contact sales</a>
 </div>
 </div>
 </div>
</section><section class="s-section s-bg-gray"><div class="s-container-narrow">
 <div class="s-header">
 <h2>Frequently Asked Questions</h2>
 <p>Everything you need to know about using the Nano Banana API</p>
 </div>
 <div class="faq-list">
 <details class="faq-item">
 <summary class="faq-q">
 <span>What model is Nano Banana?</span>
 <span class="faq-chev">▾</span>
 </summary>
 <div class="faq-a">
 <p>Nano Banana is an alias wrapper for Google Gemini image generation models. nano-banana corresponds to Gemini 2.5 Flash Image, nano-banana-2-lite corresponds to Gemini 3.1 Flash Lite Image (1K only, fast image generation), nano-banana-2 corresponds to Gemini 3.1 Flash Image (Pro-level quality + Flash speed), and nano-banana-pro corresponds to Gemini 3 Pro Image. We provide a simpler interface and lower prices.</p>
 </div>
 </details>
 <details class="faq-item">
 <summary class="faq-q">
 <span>How does pricing work?</span>
 <span class="faq-chev">▾</span>
 </summary>
 <div class="faq-a">
 <p>Pay as you go, with no subscription fee. nano-banana and nano-banana-2-lite models start at $0.0133/request, nano-banana-2 models start at $0.0267/request, and nano-banana-pro models start at $0.0333/request. Task status polling is always free. Bulk packages offer discounts of up to 27%.</p>
 </div>
 </details>
 <details class="faq-item">
 <summary class="faq-q">
 <span>What image operations are supported?</span>
 <span class="faq-chev">▾</span>
 </summary>
 <div class="faq-a">
 <p>Two operation modes: Generate (text-to-image) and Edit (multi-image editing). Generate supports 7 aspect ratios (1:1, 3:2, 2:3, 16:9, 9:16, 4:3, 3:4), and Pro models also support 1K/2K/4K resolution options. Edit mode supports uploading up to 10 images for combined editing.</p>
 </div>
 </details>
 <details class="faq-item">
 <summary class="faq-q">
 <span>How should I handle longer generation times?</span>
 <span class="faq-chev">▾</span>
 </summary>
 <div class="faq-a">
 <p>Two methods: (1) Use callback_url—set a Webhook URL, and we will POST the result when complete. (2) Poll via /nano-banana/tasks—this endpoint is free, and you can check the status at any time.</p>
 </div>
 </details>
 <details class="faq-item">
 <summary class="faq-q">
 <span>Are image URLs permanently valid?</span>
 <span class="faq-chev">▾</span>
 </summary>
 <div class="faq-a">
 <p>Yes. The returned image_url is stored on our CDN and is permanently accessible, so it can be used directly in production environments.</p>
 </div>
 </details>
 <details class="faq-item">
 <summary class="faq-q">
 <span>Can it be used with Claude or ChatGPT?</span>
 <span class="faq-chev">▾</span>
 </summary>
 <div class="faq-a">
 <p>Yes! We provide an MCP Server (mcp-nano-banana) and a Dify plugin, which can integrate directly with Claude Desktop, VS Code, and Dify workflows. Your AI Agent can generate and edit images through natural language.</p>
 </div>
 </details>
 <details class="faq-item">
 <summary class="faq-q">
 <span>How do I write a good Prompt?</span>
 <span class="faq-chev">▾</span>
 </summary>
 <div class="faq-a">
 <p>Recommended structure: subject + atmosphere + lighting + lens + texture keywords. For example: "white porcelain coffee cup, morning-light windowsill, 85mm portrait lens, shallow depth of field, soft highlights, soothing, clean, relaxed." The more specific the description, the better the generated result.</p>
 </div>
 </details>
 <details class="faq-item">
 <summary class="faq-q">
 <span>What should I keep in mind for Edit mode?</span>
 <span class="faq-chev">▾</span>
 </summary>
 <div class="faq-a">
 <p>Edit mode requires passing 1-10 images through the image_urls parameter (HTTP/HTTPS URL or Base64). Each image can be up to 10MB. The Prompt needs to describe how to process these images, for example, "make this person wear this T-shirt."</p>
 </div>
 </details>
 </div>
 </div></section><section class="s-section s-bg-white">
 <div class="s-container">
 <div class="s-header">
 <h2>Other AI Models</h2>
 <p>Explore our complete AI API suite, covering images, videos, music, and more</p>
 </div>
 <div class="rel-grid">
 <a href="https://platform.acedata.cloud/services/seedream" class="rel-card">
   <div class="rel-icon">🌌</div>
   <div class="rel-info">
     <h3>Seedream API</h3>
     <p>ByteDance high-definition text-to-image model</p>
   </div>
   <span class="rel-arrow">→</span>
 </a>
 <a href="https://platform.acedata.cloud/services/flux" class="rel-card">
 <div class="rel-icon">✨</div>
 <div class="rel-info">
 <h3>Flux API</h3>
 <p>Fast AI image generation with support for multiple styles and models</p>
 </div>
 <span class="rel-arrow">→</span>
 </a>
 <a href="https://platform.acedata.cloud/services/luma" class="rel-card">
 <div class="rel-icon">🎬</div>
 <div class="rel-info">
 <h3>Luma API</h3>
 <p>Create AI-generated videos using Dream Machine and Ray models</p>
 </div>
 <span class="rel-arrow">→</span>
 </a>
 <a href="https://platform.acedata.cloud/services/suno" class="rel-card">
 <div class="rel-icon">🎵</div>
 <div class="rel-info">
 <h3>Suno API</h3>
 <p>AI music generation—create full songs, covers, and instrumental music</p>
 </div>
 <span class="rel-arrow">→</span>
 </a>
 </div>
 </div>
</section>
<section class="nb-cta">
 <div class="s-container-narrow">
 <h2>Start Generating AI Images Now</h2>
 <p>As low as $0.0133 per call—lower prices than the official service, a simpler interface, and higher concurrency support. Pay as you go—no subscription fees, no commitments.</p>
 <div class="cta-actions">
 <a href="https://platform.acedata.cloud/documents/nano-banana-images" class="btn-cta-light">📄 View Documentation →</a>
 </div>
 </div>
</section></div>

## Quick Start

- Base URL: [https://api.acedata.cloud](https://api.acedata.cloud)
- Service page: [Nano Banana Image Generation on Ace Data Cloud](https://platform.acedata.cloud/service/nano-banana)
- Docs: [Developer documentation](https://platform.acedata.cloud/documents/nano-banana)
- Demo: [Try the demo](https://studio.acedata.cloud/nanobanana)

```bash
curl --request POST "https://api.acedata.cloud/nano-banana/images" \
  --header "Authorization: Bearer YOUR_API_KEY" \
  --header "Content-Type: application/json" \
  --data '{}'
```

## APIs and Guides

Explore the supported endpoints and integration guides for Nano Banana Image Generation.

| API | Path | Integration Guidance |
| ---- | ---- | ------------ |
| [Nano Banana Images API](https://platform.acedata.cloud/documents/23985a11-d713-41d1-ad84-24b021805b3d) | `/nano-banana/images` | [Nano Banana Images API Integration Guide](https://platform.acedata.cloud/documents/2fb479f8-63ec-424c-a93e-b12cd4250f9e) |
| [Nano Banana Tasks API](https://platform.acedata.cloud/documents/617810f5-081f-4866-a21a-cededecb0ccd) | `/nano-banana/tasks` | [Nano Banana Tasks API Integration Guide](https://platform.acedata.cloud/documents/e01ef840-3158-4eec-a6e7-337dada8d155) |

## Related Resources

- [Ace Data Cloud Developer Platform](https://platform.acedata.cloud)
- [Ace Data Cloud Docs](https://docs.acedata.cloud)
- [Status Page](https://status.acedata.cloud)
- [Ace Data Cloud GitHub Organization](https://github.com/AceDataCloud)

## Support

If you meet any issue, please check [support info](https://platform.acedata.cloud/support) or browse the latest documentation on [docs.acedata.cloud](https://docs.acedata.cloud).