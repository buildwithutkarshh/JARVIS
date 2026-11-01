JARVIS VISION 3D
A single-file, Iron Man–style holographic AI assistant that runs in your browser. A 3D hologram of Iron Man (waist up), a sci-fi terminal, voice replies, and an AI brain powered by the Gemini API.
No build step, no server, no install. Just one index.html.
Features
3D hologram bust with a custom shader: rim glow, scanlines, flicker, glitch bursts and a moving scan sweep
Boot-up animation: the hologram scans in from the bottom up
Drag to rotate, scroll or pinch to zoom
Secure terminal UI with quick-action buttons and command history
Voice replies using the browser's built-in speech synthesis
AI chat through the Gemini API: type any question and JARVIS answers (replies in the same language you write, Hinglish included)
Responsive: the hologram automatically fits above the terminal on phones and laptops
Run it
Option 1: open the file
Download index.html and double-click it (Chrome or Edge recommended). An internet connection is needed for Three.js and fonts.
Option 2: GitHub Pages (works on phones too)
Go to Settings → Pages
Choose your branch and the / (root) folder, then save
Open the link GitHub gives you: https://<utkarsh>.github.io/<JARVIS>/
Set up the AI brain (free)
Get a free API key from Google AI Studio
Open the app and press the boot button
In the terminal type:
key YOUR_API_KEY
Ask anything, for example hello
Your key is stored only in your own browser (localStorage). It is never written into the code. Do not paste your key into the source, an issue, or a commit.
Commands
Command
What it does
status
System integrity check
diagnostics
Toggle diagnostics sweep
workplace
Open the holographic workplace panels
scan
Perimeter scan
rotate
Pause or resume auto-rotation
close
Close the workplace
clear
Clear the terminal
help
List commands
key YOUR_KEY
Save your Gemini API key (key clear removes it)
model NAME
Change the Gemini model (default: gemini-flash-latest)
anything else
Sent to Gemini as a question
Privacy notes
Messages you type are sent to Google's Gemini API.
On the Gemini free tier, Google may use inputs and outputs to improve its products. Don't send passwords or private information.
Linking a billing account to your API project moves it off the free tier.
Tech
Three.js r128 (WebGL)
Custom GLSL hologram shader
Web Speech API (speech synthesis)
Gemini API (generateContent)
Plain HTML, CSS and JavaScript in one file
Credits and license
3D model: "Iron Man" by Grant Riley, from Sketchfab, licensed under CC BY-NC 4.0. The model was cropped at the waist and compressed for this project.
Because of the model's license, this project is for non-commercial use only. Attribution to the original author is required.
Iron Man and JARVIS are trademarks of Marvel. This is a fan project and is not affiliated with or endorsed by Marvel or Disney.
Roadmap
[ ] Voice input (speak to JARVIS)
[ ] Hologram reacts to the AI state (thinking, speaking)
[ ] Memory (remember name and preferences)
[ ] Hand-gesture control with webcam
[ ] Real actions through a small local server
