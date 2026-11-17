# YouTube Creator Analytics Dashboard — Wander Slowly

[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue?style=for-the-badge&logo=github)](https://mrchandrayee.github.io/you-tube-creator-analytics-dashboard/)
[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org) [![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org) [![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](./LICENSE)

A responsive, no-build dashboard reconstructed from the supplied 5.17-second screen recording.

## Visible branding and sections
- Servo / Wander Slowly creator workspace
- Studio: Overview, Content, Analytics, Planner
- Earn: Revenue, Shop
- People: Community
- Settings and Help
- Creator profile: Marta Silva / @wander.slowly

## Dashboard overview
- Greeting: “Good morning, Marta”
- Latest upload: “A slow Sunday in Alfama”
- Video metrics: 40.3k views, 7.4% click-through, 9:27 average view, 2,043 likes
- Retention indicator: 65% still watching at 7:44
- Live viewers: 1,477, with recent video list
- Summary cards: 128.5k subscribers, 1.03M views, 56,090 h watch time, €7,792 earnings

## Recreated modules and interactions
- **Analytics:** Audience / Reach / Engagement tabs, age chart, country ranking, device mix, viewer activity heatmap
- **Revenue:** Earnings / Payouts / Brand deals tabs, four revenue streams, multi-series earnings chart, payout and deal tables
- **Shop:** Product cards, product visibility toggles, stock increments, Orders tab, Add product form
- **Content:** Published video list
- **Planner:** Upcoming publishing schedule
- **Community:** Member and comment summaries
- **Settings / Help:** Workspace overview and help topics
- Global create menu, search dialog, sidebar collapse and light/dark appearance toggle

## Run locally
No npm, framework or build process required. Extract the ZIP and open `index.html` in a modern browser.

Or run:
```bash
python3 -m http.server 8000
```
Then visit http://localhost:8000.

## Source-code fragments visible in the recording
The code preview shown in the video contains a TSX snippet from `src/App.tsx`, including:
- `const D = 0.62, E = 'power3.inOut';`
- `const vis = { v: on ? W : R };`
- `side.style.setProperty('--vis', `${vis.v}px`);`
- `side.style.clipPath = `inset(0 ${W - vis.v}px 0 0 round 28px)`;`
- `const st = Flip.getState(movers());`
- `swap(); paint();`
- `gsap.to(vis, { v: on ? R : W, duration: D, ease: E, onUpdate: paint });`
- `gsap.fromTo(col, { paddingLeft: padFrom }, { paddingLeft: padTo, duration: D, ease: E });`
- `Flip.from(st, { targets: movers(), duration: D, ease: E });`
- `gsap.from(words(), { opacity: 0, x: -10 }, { opacity: 1, x: 0, stagger: 0.018, delay: D * 0.4 });`

The source recording does not show the complete original repository. The delivered project is a runnable vanilla HTML/CSS/JS reconstruction of the visible product UI and interactions, not a byte-for-byte extraction of unseen source. Sample analytics, revenue, products and people are demonstration data. No YouTube account, analytics API, payouts or commerce backend is connected.

## 👨‍💻 Author

**mrchandrayee** · [GitHub](https://github.com/mrchandrayee)

## 📄 License

[MIT License](./LICENSE)
