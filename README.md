# Engineer Mission Control

**Engineers are mission control. Doctors are the failed spacecraft.**

A Hinglish satire website where an engineer ragebaits a doctor. It looks like a white-and-pink mission control room. Engineer-1 reaches orbit, Doctor-1 says "dekhte hain" and crashes, and the doctor's blood pressure climbs live while you scroll.

> Satire hai. Doctors, aap bhi great ho. Bas handwriting…

**Live site:** https://aadeshthe-coder.github.io/doctormads/ (once GitHub Pages is switched on, see [Deploy](#deploy))

## What's on the page

- **Live launch.** After a countdown, Engineer-1 flies a clean gravity turn to a 408 km orbit. Doctor-1 coughs "gas hai", flames out about 11 m up and tips over. Telemetry and a mission log update as it happens. **Phir launch karo** replays it.
- **3D orbit background.** A pink planet with Engineer-1 cruising its orbit while Doctor-1 tumbles and leaks smoke below its dotted "planned" orbit. Scrolling flies the camera around the planet.
- **Crew vitals.** Doctor-1's BP monitor rises the more you scroll, laugh and roast. The screen edges glow red as it climbs. You can switch it between mmHg and kPa.
- **Go / no-go checklist.** Six reasons engineers are superior, on a 3D ring that turns as you scroll.
- **Meme portfolio.** Nine classic internet formats, redrawn as animated CSS and SVG: Nahi/Haan, Nobody, Expanding brain, Two buttons, Always has been, Deewaar dialogue, They don't know, Rishtedaar logic, and a prescription CAPTCHA. Each one has filters and a 😂 counter.
- **Comms with Doctor-1.** A five-round chat where you pick the comeback. The roast meter ranks you, up to CTO (Chief Taunt Officer).
- **Rescue packages, anomaly desk and a 404.**
  - Plans are Low Orbit, Moon Mission and Mars. Mars is "not found".
  - Every complaint filed at the anomaly desk gets rejected.
  - The "Why doctors are better" button opens a 404.

Easter egg: type `gas` anywhere on the page.

## Run it locally

The whole site is one file, `index.html`. Open it in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000. You need an internet connection, because the libraries and fonts load from cdnjs and Google Fonts.

## Deploy

**GitHub Pages**
1. In this repository, go to **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Pick `main` and `/ (root)`, then save.

After a minute the site is live at the link above.

**Netlify**
1. Log in at [app.netlify.com](https://app.netlify.com) first.
2. Drag this folder onto the **Sites** page.

Sites dropped without logging in are temporary and get deleted.

## Settings and troubleshooting

- The **Animations band karo** button at the bottom of the page turns all motion off, and back on. The browser remembers the choice.
- Add `#debug` to the end of the link to see what the browser supports: libraries, WebGL, frame rate and the reduce-motion setting. This helps when something doesn't animate on a phone.
- The footer shows the build number (currently v10). Use it to check that a phone isn't showing an old cached copy.

## Built with

- Plain HTML, CSS and JavaScript. There is no build step and nothing to install.
- [three.js](https://threejs.org/) r128 for the 3D orbit.
- [GSAP](https://gsap.com/) 3.12.5 with ScrollTrigger for the scroll animation and the launch sequence.
- Google Fonts: Unbounded, Hanken Grotesk, IBM Plex Mono, Anton and Kalam.

`index.html` is a generated, self-contained build with all the CSS and JavaScript inlined. Edit it directly, or rebuild it from the separate source files.

## Notes

- The memes use well-known internet formats, but every drawing and joke here is original. No meme images are copied.
- The BP monitor is fake. If your BP really is this high, see a doctor. Kisi aur ko.
- This is satire, made for laughs. It is not medical advice.
