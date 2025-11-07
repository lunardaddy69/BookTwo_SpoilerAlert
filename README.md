Here’s a clean, Markdown-formatted README.md that will look great directly on your GitHub repository page for this feature.
It’s concise, readable, and explains the structure without dumping code.

⸻

Mariana Book Two Spoiler Reveal Block

This feature adds an interactive spoiler-protected synopsis section for Mariana Book Two on the author’s website.
It hides the text behind a blurred overlay until the visitor clicks to reveal it.

⸻

✨ Features
	•	Blurred preview: The synopsis text is visible but unreadable until revealed.
	•	Hover overlay: Displays a dark overlay with a message warning of spoilers.
	•	Click to reveal: Removes the blur and overlay, revealing the text in the site’s normal font and color.
	•	Automatic styling: Uses existing site typography and color palette for seamless integration.
	•	Lightweight: Uses only vanilla HTML, CSS, and JavaScript (no external libraries).

⸻

🧩 Structure Overview
	•	HTML:
  	•	A wrapper <div> contains the spoiler block.
  	•	Inside are two layers:
    	•	.mariana-spoiler-overlay → displays the “Book Two Synopsis Contains Spoilers for Book One – Click to Reveal” message.
    	•	.mariana-spoiler-text → contains the actual synopsis text.
  	•	CSS:
    	•	.mariana-spoiler-text is blurred and lightened until revealed.
    	•	Hovering over the block fades in the overlay.
    	•	Clicking removes the blur and hides the overlay.
	•	JavaScript:
  	•	Adds a revealed class to the spoiler block when clicked, triggering the CSS transitions.

⸻

🛠️ Usage
	1.	Copy the entire code snippet from this repository.
	2.	Paste it into a Squarespace Code Block (or any HTML page).
	3.	Adjust the synopsis text, colors, or blur intensity if needed.
  	•	Increase blur(6px) for a heavier blur.
  	•	Adjust overlay text in the <div class="overlay-text">.

⸻

🎨 Customization Tips
	•	To change the brightness of the hidden text, edit the color property in:
      .mariana-spoiler-text {
        color: hsla(43, 100%, 90%, 0.8);
      }
	•	To change the reveal color (normal state), modify:
      .mariana-spoiler-block.revealed .mariana-spoiler-text {
        color: hsla(43, 0%, 100%, 0.9);
      }
	•	The overlay message text can be edited directly inside the HTML.
