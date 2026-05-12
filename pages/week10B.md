---
title: 10B) AI prompt for differentiated question set
layout: page

parent: 10) Inclusive digital learning resource
nav_enabled: true
nav_order: 5
---

## Week 10 AI Task

### Prompt
```
I created the following inclusive quiz page "        
<h1>🛠️ CAD vs CAM: Workshop Design & Manufacturing</h1>

<div class="time-guide">
    ⏱️ <strong>5–8 minute activity</strong> — Read the facts, answer 5 questions using different response styles, then review feedback.
</div>

<div class="format-key">
    <span>📌 <strong>Varied response formats per question</strong> (UDL: multiple means of action & expression)</span>
    <span class="badge">🎤 Audio + ✏️ Typing</span>
    <span class="badge">✅ Multiple-select + 😀 Emojis</span>
    <span class="badge">🔘 Single-select + 🎨 Emojis</span>
</div>

<!-- Q1: Typing + Audio ONLY (no radio) -->
<div class="quiz-card">
    <div class="mini-lesson">
        📘 <strong>Quick fact:</strong> CAD (Computer‑Aided Design) lets you create 2D drawings and 3D models before cutting any material.
    </div>
    <div class="question-text">1️⃣ Name one specific way CAD helps a metal or timber workshop save money or time.</div>
    <div class="response-area">
        <div class="method-label">✏️ Option 1: Type your answer</div>
        <textarea rows="2" placeholder="e.g., 'It reduces material waste by nesting parts' or 'You can test designs virtually'..." class="answer-text" data-q="1"></textarea>
        <br/><br/>
        <div class="method-label">🎙️ Option 2: Record a spoken answer</div>
        <div class="audio-controls">
            <button class="record-btn" data-q="1">🎤 Start Recording</button>
            <button class="stop-btn" data-q="1" disabled>⏹️ Stop</button>
            <audio controls class="playback" data-q="1" style="display:block; margin-top:6px;"></audio>
        </div>
    </div>
    <div class="feedback" id="feedback-1"></div>
</div>

<!-- Q2: Multiple-select checkboxes + EMOJIS   -->
<div class="quiz-card">
    <div class="mini-lesson">
        📘 <strong>Quick fact:</strong> CAD can do more than just drawing — it can simulate stress, generate cutting lists, and create photo‑realistic renders.
    </div>
    <div class="question-text">2️⃣ Which of these are actual uses of CAD in manufacturing? <span style="font-size:0.9em;">(✅ Select ALL that apply — more than one correct)</span></div>
    <div class="response-area">
        <div class="method-label">✅ Multiple-select (check all that are true)</div>
        <label class="emoji-option"><input type="checkbox" name="q2" value="3D modelling"> 🧊 3D modelling</label><br>
        <label class="emoji-option"><input type="checkbox" name="q2" value="Generating cutting lists"> 📋 Generating cutting lists </label><br>
        <label class="emoji-option"><input type="checkbox" name="q2" value="Ordering coffee"> ☕ Ordering coffee for the workshop </label><br>
        <label class="emoji-option"><input type="checkbox" name="q2" value="Stress analysis"> ⚙️ Virtual stress / strength analysis</label><br>
        <label class="emoji-option"><input type="checkbox" name="q2" value="Painting finished goods"> 🎨 Painting finished products</label>
      <br/><br/>
        
        <div class="method-label">🎙️ Alternative: Record a spoken answer instead</div>
        <div class="audio-controls">
            <button class="record-btn" data-q="2">🎤 Start Recording</button>
            <button class="stop-btn" data-q="2" disabled>⏹️ Stop</button>
            <audio controls class="playback" data-q="2" style="display:block; margin-top:6px;"></audio>
        </div>
    </div>
    <div class="feedback" id="feedback-2"></div>
</div>

<!-- Q3: Typing + Audio ONLY (open-ended on CAD vs CAM) -->
<div class="quiz-card">
    <div class="mini-lesson">
        📘 <strong>Quick fact:</strong> CAM (Computer‑Aided Manufacturing) takes CAD files and turns them into machine instructions (G‑code) for CNC routers, laser cutters, and mills.
    </div>
    <div class="question-text">3️⃣ In your own words, what is the MAIN difference between CAD and CAM?</div>
    <div class="response-area">
        <div class="method-label">✏️ Type your answer</div>
        <textarea rows="2" placeholder="e.g., 'CAD is for design, CAM is for automated cutting/machining'..." class="answer-text" data-q="3"></textarea>
        <br/><br/>
        <div class="method-label">🎙️ Record your spoken explanation</div>
        <div class="audio-controls">
            <button class="record-btn" data-q="3">🎤 Start Recording</button>
            <button class="stop-btn" data-q="3" disabled>⏹️ Stop</button>
            <audio controls class="playback" data-q="3" style="display:block; margin-top:6px;"></audio>
        </div>
    </div>
    <div class="feedback" id="feedback-3"></div>
</div>

<!-- Q4: Single-select radio buttons + EMOJIS -->
<div class="quiz-card">
    <div class="mini-lesson">
        📘 <strong>Quick fact:</strong> A CNC router can cut timber, aluminium, and plastics — but it needs CAM software to tell it where to move.
    </div>
    <div class="question-text">4️⃣ What does CAM add that CAD alone cannot do? (Choose ONE best answer)</div>
    <div class="response-area">
        <div class="method-label">🔘 Select one answer (with emojis)</div>
        <label class="emoji-option"><input type="radio" name="q4" value="Draw pretty pictures"> 🎨 Draw pretty pictures </label><br>
        <label class="emoji-option"><input type="radio" name="q4" value="Control CNC machines automatically"> 🤖 Control CNC machines </label><br>
        <label class="emoji-option"><input type="radio" name="q4" value="Sharpen drill bits"> 🔧 Sharpen drill bits</label><br>
        <label class="emoji-option"><input type="radio" name="q4" value="Measure timber moisture"> 🌲 Measure timber moisture</label>
        <br/><br/>
        <div class="method-label">🎙️ Or record your spoken answer</div>
        <div class="audio-controls">
            <button class="record-btn" data-q="4">🎤 Start Recording</button>
            <button class="stop-btn" data-q="4" disabled>⏹️ Stop</button>
            <audio controls class="playback" data-q="4" style="display:block; margin-top:6px;"></audio>
        </div>
    </div>
    <div class="feedback" id="feedback-4"></div>
</div>

<!-- Q5: Typing + Audio ONLY (real-world application) -->
<div class="quiz-card">
    <div class="mini-lesson">
        📘 <strong>Quick fact:</strong> Many modern workshops use CAD + CAM together — design on screen, then cut on a CNC machine without manual measuring.
    </div>
    <div class="question-text">5️⃣ Describe ONE real-world project where you would use BOTH CAD and CAM. (e.g., a piece of furniture, metal bracket, sign, etc.)</div>
    <div class="response-area">
        <div class="method-label">✏️ Type your example</div>
        <textarea rows="2" placeholder="e.g., 'Design a wooden cabinet in CAD, then use CAM to cut the panels on a CNC router'..." class="answer-text" data-q="5"></textarea>
        <br/><br/>
        <div class="method-label">🎙️ Record your spoken example</div>
        <div class="audio-controls">
            <button class="record-btn" data-q="5">🎤 Start Recording</button>
            <button class="stop-btn" data-q="5" disabled>⏹️ Stop</button>
            <audio controls class="playback" data-q="5" style="display:block; margin-top:6px;"></audio>
        </div>
    </div>
    <div class="feedback" id="feedback-5"></div>
</div>

<button class="submit-btn">📥 Submit & Get Feedback</button>

<!-- Transcript for UDL princples etc.-->
<div class="transcript">
    <h3>📄 Accessibility & Transcript Information</h3>
    <p><strong>Visual description:</strong> Each question card has a coloured top border, a light orange fact box, and a alternative background colour for response types areas. Buttons are labelled clearly. Emojis accompany options for visual support.</p>
  <p>All questions and text can be read with a screenreader, and conforms to colour constrast requirements (checked using the Lighthouse plugin - scoring 100% accessibiltity and best practice)</p>
    <p><strong>Expected audio/text answers (guide for markers / readers of this portfolio):</strong></p>
    <ul>
        <li><strong>Q1:</strong> Reduces waste, virtual testing, faster revisions, accurate cutting lists.</li>
        <li><strong>Q2:</strong> Correct checkboxes: 3D modelling, cutting lists, stress/strength analysis. Coffee and painting are wrong.</li>
        <li><strong>Q3:</strong> CAD = design/drawing; CAM = manufacturing/machine control.</li>
        <li><strong>Q4:</strong> Control CNC machines.</li>
        <li><strong>Q5:</strong> Any valid example: cabinet, sign, engine bracket, furniture, etc.</li>
</div>"It is a digital learning resource is an introductory HTML quiz on CAD and CAM, designed for a Stage 4 (Years 7–8) Technology or Industrial Technology class studying metalwork or engineering before starting content of Computer Aided Design tools. Can you look at the hints, and quiz questions and generate two more versions of this quiz, one that uses more technical terms and references and one that we could use with a younger audience (for example a stage 2 class using TinkerCAD for the first time, but wanting to cover information about how CAM is different to CAD etc. still in a suitable way). Just the lists of questions, and answers for these two cohorts will be best (rather than attempting to generate whole pages of HTML)
```

### Response

Here are two adapted versions of the quiz questions and answers, keeping the same core 5-question structure but tailoring the language, hints, and concepts for each cohort.

---

### Version 1: Advanced / Technical (Stage 5–6 or VET)
**Cohort:** Years 9–12, Industrial Technology (Metal/Timber), Engineering Studies, or VET Certificate II in Engineering.
**Focus:** Precision, workflows, terminology (G-code, post-processor, tolerances), and efficiency.

| Q# | Question | Acceptable Answers (Technical) |
| :--- | :--- | :--- |
| **1** | Name one specific way CAD assists with **cost reduction or lead time minimisation** in a CNC machining or fabrication workshop. | - "Using simulation to detect collisions before cutting."<br>- "Generating accurate flat patterns for sheet metal nesting to reduce offcuts."<br>- "Automatically creating Bills of Materials (BOM) for procurement before production starts." |
| **2** | Which of these are **core outputs or capabilities** of modern CAM software? (Select ALL that apply) | ✅ **Post-processing G-code** (converts toolpaths to machine language)<br>✅ **Toolpath simulation** (verifying cutter moves before machining)<br>✅ **Feed rate optimisation** (adjusting speed based on material)<br>❌ *Generating 3D renders* (That’s CAD)*<br>❌ *Drawing blueprints* (That’s CAD)* |
| **3** | Explain the key **data exchange** difference between CAD and CAM. What does one produce that the other consumes? | - "CAD produces a **geometric model** (STEP, IGES, STL). CAM consumes that model and produces **machine instructions** (G-code, M-code)."<br>- "CAD is the *what* (shape), CAM is the *how* (cutting strategy)." |
| **4** | If a CNC mill has a **5-axis head** but the CAM software is only licensed for 3-axis, what is the practical limitation? | - "The CAM software cannot generate toolpaths that tilt the cutter head, so you cannot machine undercuts or complex 3D contours."<br>- "You lose simultaneous axis control, forcing more setups." |
| **5** | Describe a **real-world manufacturing scenario** where you would use CAM **for adaptive machining** (not just code generation). | - "Using a probe + CAM to scan a rough casting, then automatically adjusting toolpaths to machine the *actual* material shape."<br>- "CAM with rest machining – to automatically remove leftover stock from a roughing pass using a smaller tool." |

---

### Version 2: Younger / Introductory (Stage 2 – Years 3–4)
**Cohort:** Primary school students (e.g., using TinkerCAD for the first time).
**Focus:** Basic concepts of "design on computer" vs. "computer helps make it", using simple analogies (digital LEGO, robot helpers).

| Q# | Question | Acceptable Answers (Simple Language) |
| :--- | :--- | :--- |
| **1** | Before you build something with real wood or plastic, how can drawing it on a computer (CAD) help you **save materials**? | - "You can see if pieces fit together without wasting real wood."<br>- "You can copy and paste shapes so you don't cut extras by mistake."<br>- "You can make it bigger or smaller without re-cutting." |
| **2** | Pick ALL the things you can do with **3D design software** like TinkerCAD. (Select ALL that apply) | ✅ **Stack shapes** (like digital blocks)<br>✅ **Change colours** of your design<br>✅ **Zoom and rotate** to look at your model from all sides<br>❌ *Actually cut real wood* (The computer can’t cut – that’s for a machine)<br>❌ *Eat your design for lunch* |
| **3** | If CAD is **designing** on a screen, what does CAM do that is **different**? (HINT: It uses a machine) | - "CAM uses a machine to cut or print your design."<br>- "CAD is drawing, CAM is building."<br>- "CAM tells a robot or 3D printer where to move." |
| **4** | Which job does a **CAM machine** (like a CNC router or laser cutter) do that your computer cannot do alone? (Choose ONE best answer) | - "Actually cut the wood or plastic."<br>- "Hold the material in place while cutting."<br>- "Make real dust and noise." |
| **5** | Name a **real object** you could design in TinkerCAD (CAD) and then cut or print using a CAM machine. | - "A name tag for my school bag."<br>- "A phone stand."<br>- "A cookie cutter shape."<br>- "A toy car body." |
| **Bonus (optional)** | What is your favourite **emoji** to describe how a CNC machine sounds? | - 🤖 (robot) – *for the beeping*<br>- 🎵 (musical notes) – *for the cutting sound*<br>- 😴 (sleepy) – *if it's slow* |

Would you like me to turn either of these versions into a full HTML quiz page, or create a printable worksheet from them?