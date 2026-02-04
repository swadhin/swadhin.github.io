# Website Design & Update Guide

This document captures all design decisions, content preferences, and technical specifications for swadhinpradhan.com. Use this as a reference for future updates.

---

## Site Overview

**Owner:** Swadhin Pradhan  
**Role:** ML Tech Lead @ Cisco  
**Focus Areas:** Wireless Sensing, GenAI for Networks, Indoor Air Quality, Mobile Systems Research  
**Domain:** www.swadhinpradhan.com (GitHub Pages)

---

## Design Philosophy

### Core Principles
- **Idea-centric, not CV-style** - Focus on research themes and vision, not just listing papers
- **Simple and fast loading** - Pure HTML/CSS/JS, no frameworks, < 20KB target
- **No scrolling needed** - Tabbed interface, everything fits in viewport
- **Recruiter and LLM friendly** - Optimized for search engines and AI indexing
- **Modern but professional** - Clean, minimal design without being flashy

### Tech Stack
- Pure HTML5 + CSS3 + vanilla JavaScript
- System fonts (no external font files)
- Inline SVG favicon
- No build tools or frameworks
- GitHub Pages hosting

---

## Site Structure

### Hero Section
```
[Photo] Swadhin Pradhan
        ML Tech Lead @ Cisco
        [Email] [Scholar] [CV]
        
        [Bio paragraph - 3-4 sentences]
```

**Photo:** Circular, 80px, with `object-position: center 15%` to show face properly

**Bio:** Full sentences, no bold formatting. Currently:
> "I build AI systems that perceive and act in the physical world. My work spans wireless sensing using RFID, mmWave, and acoustics, GenAI for network intelligence, indoor air quality monitoring, and mobile systems research. I hold a PhD from UT Austin, have published 15+ papers at premier venues including MobiCom, CHI, SenSys, and NeurIPS, and shipped multiple AI products at Cisco."

**Special formatting:**
- "PhD" is hyperlinked to `papers/PRADHAN-DISSERTATION-2020.pdf`
- No mention of patents in bio (patents section exists separately)

**Links order:** Email → Scholar → CV (no GitHub in hero)

### Tabs (4 tabs)
1. **Wireless Sensing** - Research on RFID, mmWave, acoustic sensing
2. **GenAI for Networks** - Industry work at Cisco
3. **Indoor Air Quality** - Environmental sensing research
4. **Mobile Systems** - Mobile computing, authentication, notifications, energy optimization

### Tab Content Structure
Each tab has:
1. **Idea intro** (1-2 sentences in a styled box explaining the vision)
2. **Project cards** (grid of projects with venue badges and links)

---

## Content Guidelines

### Language Preferences
- Use "we" for collaborative work descriptions (not "I" in idea sections)
- Use full sentences, not fragments
- Keep project hooks concise (1 line)
- Don't use bold formatting in bio paragraph

### Project Card Format
```
[Project Name]     [Venue Badge]
One-line hook describing the work
[PDF] [PPT] [BibTeX] [Video] [Code] [Dataset] [Patent]
```

### Venue Badge Colors
- MobiCom: Blue (#3b82f6)
- CHI: Green (#10b981)
- SenSys: Orange (#f59e0b)
- UbiComp: Purple (#8b5cf6)
- IPSN: Red (#ef4444)
- MobiHoc: Pink (#ec4899)
- INFOCOM: Cyan (#06b6d4)
- NeurIPS: Orange (#f59e0b)
- Upcoming: Orange (#f97316)
- Other/Patents: Gray (#6b7280)

---

## Tab 1: Wireless Sensing

### Idea Text
> "Building multi-modal intelligent sensing systems. Using RFID, acoustic signals, and mmWave radar, we build multimodal sensing systems that track motion, measure temperature, recognize gestures, and authenticate users—enabling embodied intelligence without cameras or wearables. This is for the next generation of robotics and smart environments."

### Projects (in order)
1. MIRO (SenSys'26) - "Worker safety using multi-radar re-identification"
2. MARS (IPSN'24) - "Track multiple people's activities using mmWave"
3. TIMU (MobiHoc'21) - "Sense ball rotation using passive RFID tags"
4. RTSense (SenSys'20) - "Battery-free temperature sensing with RFID"
5. RTrack (MobiCom'19) - "Room-scale hand tracking via sound"
6. REVOLT (UbiComp'19) - "Stop voice replay attacks on smart assistants"
7. SAMS (UbiComp'18) - "Map indoor spaces using phone speakers"
8. RIO (MobiCom'17) - "Touch gestures on any surface via RFID Tags"
9. Konark (WPA'17) - "RFID-based seamless checkout for retail stores"

### Excluded from this tab
- ActivPass (CHI'15) - moved to Mobile Systems
- Notification (INFOCOM'17) - moved to Mobile Systems

---

## Tab 2: GenAI for Networks

### Idea Text
> "GenAI for real-world systems. Networks generate massive multimodal data—packets, logs, configs. We're building foundation models that understand this "language," enabling AI to diagnose problems, predict failures, and act autonomously. We are shipping AI products at scale, from foundational generative models for networks to agentic diagnostics."

### Projects (in order, with links)
1. **Cisco AI Assistant** - RAG + LLM driven assistant → [Learn more](https://www.cisco.com/site/us/en/solutions/artificial-intelligence/ai-assistant/index.html)
2. **Large Packet Model (LPM)** - Training LLMs on network packets (no external link - internal)
3. **Sherlock** - GenAI-powered PCAP analysis → [AI PCAP Analyzer](https://documentation.meraki.com/Platform_Management/Dashboard_Administration/Troubleshooting_and_Support/Troubleshooting/AI_PCAP_Analyzer)
4. **AI-RRM** - AI-driven Radio Resource Management → [AI-RRM Docs](https://documentation.meraki.com/Wireless/Operate_and_Maintain/User_Guides/Radio_Settings/AI_-_RRM)
5. **Networks Like You** - ML-driven config recommendations → [Meraki Health](https://meraki.cisco.com/blog/2021/09/use-data-to-define-your-network-with-meraki-health/)
6. "...and more in development"

### Removed from this tab
- Smart Alerting
- Intelligent RCA

---

## Tab 3: Indoor Air Quality

### Idea Text
> "Indoor pollution is invisible but impacts health daily. From CO₂ buildup in offices to particulate matter in factories, we build systems that sense, visualize, and help people act on indoor air quality—using everything from low-cost sensors to AR games."

**Note:** Use CO₂ (subscript 2), not CO2

### Projects (in order)
1. MIRO (SenSys'26) - NOT in this tab anymore, moved to Sensing
2. CO₂ AR (CHI'26) - "AR game to find and disperse indoor CO₂ hotspots"
3. DALTON (JCSS'24) - "Mapping indoor air pollution dynamics across India"
4. Air Quality Dataset (NeurIPS'24) - "Indoor air quality dataset with daily activities in low-income communities" → [Dataset](https://github.com/prasenjit52282/dalton-dataset)
5. Air Track (MobileHCI'24) - "Using air quality monitors to detect indoor occupancy"

---

## Tab 4: Mobile Systems

### Idea Text
> "Building intelligent mobile systems. From password-free authentication using daily activities to understanding notification behaviors and optimizing mobile sensing, we explore how smartphones can become smarter, more secure, and energy-efficient through context-aware computing."

### Projects (in order)
1. Notification (INFOCOM'17) - "Understanding and predicting mobile notifications"
2. ActivPass (CHI'15) - "Password-free authentication using daily activities"
3. OpTen (COMSNETS'15) - "Optimizing energy consumption in mobile sensing"
4. RetailGuide (COMSNETS'14) - "Indoor navigation using landmarks and phone sensors"
5. Sprinkler (CellNet'13) - "Efficient mobile data offloading through WiFi"

---

## Patents Section

### Structure
Two subsections:
1. **GenAI for Networks (Filed 2024-2026, Pending)** - 4 key patents + "and 5+ more"
2. **Wireless Sensing** - 2 granted patents with links

### GenAI Patents (show only these 4)
- US19270155 — Large Packet Model for Network Devices
- US19463024 — On-Device Micro-Generative Models
- US19463036 — Agentic Second-Opinion Diagnostics
- US63962037 — Hallucination Prevention for Network LLMs
- "...and 5+ more pending applications"

### Wireless Sensing Patents (with links)
- US20180157876 — RFID Touch Gestures → [Patent Link](http://www.freepatentsonline.com/y2018/0157876.html)
- WO2017131748 — Notification Scheduling → [Patent Link](https://patentscope.wipo.int/search/en/detail.jsf?docId=WO2017131748)

---

## Press Coverage Section

Located after Patents section, before Footer.

### Structure
Three projects highlighted with press coverage:
1. **RTSense** - Battery-free temperature sensing with passive RFID
2. **REVOLT** - Preventing voice replay attacks on smart speakers
3. **ActivPass** - Password-free authentication using daily activity

### Format
Each project card includes:
- Project name (hyperlinked to paper PDF)
- Brief description
- Links to press articles

### Press Links
**RTSense:**
- Paper: `papers/rtsense.pdf` (linked from project name)
- UT Austin CS News: https://www.cs.utexas.edu/news/2021/exploring-passive-rfid-tag-use-sensory-technology

**REVOLT:**
- Paper: `papers/revolt_ubicomp_swadhin.pdf` (linked from project name)
- Smart Homes Quarterly (Q2 2020): `SmartHomes-Q2-2020_v3.pdf`

**ActivPass:**
- Paper: `papers/activpass_chi_2015.pdf` (linked from project name)
- The Guardian: https://www.theguardian.com/commentisfree/2015/may/05/passwords-activpass-security-codes
- Boston Globe: https://www.bostonglobe.com/ideas/2015/05/12/one-simple-solution-for-online-passwords/WNeYN6HrVLdobXdnEA1WsN/story.html
- NDTV: https://www.ndtv.com/offbeat/bugged-with-passwords-your-daily-activity-could-help-you-log-in-1239362
- American Banker: https://www.americanbanker.com/bank-technology/authentication-advances-may-finally-kill-passwords-and-pins-1074298-1.html

---

## Footer

Simple, one line:
> © 2026 Swadhin Pradhan

**Removed:** "PhD in Computer Science, UT Austin · Previously at NEC Labs America"

---

## SEO & LLM Optimization

### Meta Tags
- Title: "Swadhin Pradhan | ML Tech Lead | Physical AI, Sensing, GenAI"
- Description: Comprehensive, includes key terms and achievements
- Keywords: Include "Physical AI", "Multimodal AI", "Embodied AI", "Robotics", etc.

### Schema.org JSON-LD
- Person type with detailed attributes
- knowsAbout array with all expertise areas
- sameAs links: GitHub, Google Scholar, LinkedIn
- BreadcrumbList for navigation

### Hidden LLM Summary
Accessible `<aside>` with:
- Core expertise list
- Achievements summary
- "Relevant For" section with recruiter-friendly job titles

### Files
- `robots.txt` - Allows all major crawlers including GPTBot, ClaudeBot, PerplexityBot
- `sitemap.xml` - Single page sitemap
- Canonical URL set

---

## Styling Preferences

### Colors (CSS Variables)
- Background: #fafafa (light), #111827 (dark mode)
- Text: #1a1a1a (light), #f9fafb (dark mode)
- Accent: #2563eb (blue)
- Cards: White with subtle border and shadow

### Favicon
Simple green circle (#10b981), inline SVG

### Typography
System font stack: `-apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif`

### Dark Mode
Automatic via `prefers-color-scheme: dark` media query

---

## JavaScript Features

### URL Hash Navigation
The site uses URL hash fragments to preserve tab state across navigation:

**How it works:**
- Clicking a tab updates the URL hash (e.g., `#sensing`, `#genai`, `#airquality`, `#mobile`)
- When user clicks a PDF link and uses browser back button, the hash is restored
- Page automatically switches to the correct tab based on hash
- Defaults to `#sensing` if no hash is present

**Implementation:**
- `switchToTab(tabId)` - Core function that handles tab switching
- `hashchange` event listener - Detects back/forward browser navigation
- Initial page load checks hash and opens correct tab

**Benefits:**
- Users return to the same tab after viewing PDFs
- Tabs are bookmarkable with direct URLs
- Browser history works as expected

---

## File References

### CV
`cvs/swadhin_cv_2026.pdf`

### Photo
`photos/swadhin_o3.jpeg` with alt text: "Swadhin Pradhan - ML Tech Lead at Cisco, PhD UT Austin, Physical AI and GenAI researcher"

### Papers Directory
`papers/` - All PDF files

### Presentations
`ppts/` - PPT/PPTX/PDF files

### BibTeX
`bibs/` - .bib files for each paper

---

## Important Notes

1. **Don't use emojis** unless explicitly requested
2. **All content must be in HTML** (not dynamically loaded) for LLM indexing
3. **Tab switching via JS with URL hash navigation** - Tabs use URL hash fragments (e.g., `#genai`, `#mobile`) to preserve state when navigating back from PDFs
4. **Links open in new tab** for external URLs (use `target="_blank"`)
5. **Stats format:** "15+ papers at premier venues including...", "4+ Cisco products shipped"
6. **Patent status:** Always clarify "filed" or "pending" for recent patents
7. **Bio formatting:** No mention of patents in bio paragraph (covered in separate Patents section)

---

## Quick Update Checklist

When updating the site:
- [ ] Update CV link if new version uploaded
- [ ] Add new papers to appropriate tab (Wireless Sensing, GenAI, Air Quality, or Mobile Systems)
- [ ] Update patent count if new filings
- [ ] Update sitemap.xml lastmod date
- [ ] Check all PDF/PPT links work
- [ ] Verify Schema.org JSON-LD is accurate
- [ ] Test on mobile and dark mode
- [ ] Test tab navigation and back button behavior
- [ ] Update AGENTS.md if making structural changes

---

## Content Organization by Tab

### Wireless Sensing
Focus: RFID, mmWave radar, acoustic sensing for physical world perception
Projects: MIRO, MARS, TIMU, RTSense, RTrack, REVOLT, SAMS, RIO, Konark

### GenAI for Networks
Focus: Foundation models for network data, AI-driven diagnostics
Products: Cisco AI Assistant, LPM, Sherlock, AI-RRM, Networks Like You

### Indoor Air Quality
Focus: Environmental sensing, air pollution monitoring
Projects: CO₂ AR, DALTON, Air Quality Dataset, Air Track

### Mobile Systems
Focus: Mobile computing, authentication, notifications, energy optimization
Projects: Notification, ActivPass, OpTen, RetailGuide, Sprinkler
