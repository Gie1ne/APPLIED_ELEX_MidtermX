# APPLIED_ELEX_MidtermX
Applied electronics midterm mock exam

# Applied Electricity Interactive Web Mock Examination

An interactive, single-file web application built to serve as a comprehensive 100-item practice examination for **Applied Electricity**. Designed strictly according to the *UP REVIEWER* study guide, this tool features automated flexible grading, dynamic input formatting, mobile-first navigation, and persistent progress saving.

---

## 📋 Table of Contents
- [Features](#-features)
- [Exam Structure](#-exam-structure)
- [Grading Engine & Tolerances](#-grading-engine--tolerances)
- [Tech Stack](#-tech-stack)
- [Getting Started & Deployment](#-getting-started--deployment)
- [Usage Instructions](#-usage-instructions)
- [Study Guide Coverage](#-study-guide-coverage)

---

## ⚡ Features

- **100-Item Full Curriculum Test**: Complete coverage strictly derived from the reference notes (Atomic Theory, AC/DC, Hazards, Ohm's/Power Law, Multimeter Parts, Circuit Testing, and 20 Electronic Devices).
- **Auto-UPPERCASE Input System**: Live input transformation enforces strict uppercase standard formatting without requiring manual Caps Lock toggling.
- **Flexible Answer Matching Engine**: Advanced string normalization handles pluralization variants (`ELECTRON` / `ELECTRONS`), alternative unit notations (`120`, `120V`, `120 VOLTS`), equation variants (`V=I*R`, `V=I X R`), and accepted term synonyms.
- **Mathematical Word Problems**: 10 calculation questions testing direct and inverse applications of Ohm's Law ($V = I \times R$) and Power Law ($P = V \times I$).
- **Mobile-First UX**: Responsive UI featuring touch-friendly navigation, sticky header controls, and a slide-out 100-question map drawer with backdrop support.
- **State Persistence**: Uses browser `localStorage` to save answer state, flagged items, active filters, and elapsed test time, preventing loss of progress on accidental refreshes.
- **Detailed Scorecard & Review Mode**: Provides an instant percentage score, 75% passing threshold verification, live timer stats, and an item-by-item answer key breakdown paired with reference excerpts.

---

## 📊 Exam Structure

| Part | Item Range | Category | Description |
| :--- | :--- | :--- | :--- |
| **Part I** | Q1 – Q50 | **Identification** | Terminology, electronic components, VOM multimeter controls, atomic structures, and hazard definitions. |
| **Part II** | Q51 – Q75 | **True or False** | Operational safety rules, human body resistance variables, circuit testing paths, and measurement rules. |
| **Part III** | Q76 – Q85 | **Calculations** | Step-by-step word problems requiring Ohm's Law ($V, I, R$) and Power Law ($P, V, I$) formulas. |
| **Part IV** | Q86 – Q100 | **Enumeration & Short Answer** | Specific numeric quantities, temperature limits, AC wave degree metrics, pinouts (Pins 2 & 7, A1–A2), and indicator colors. |

---

## 🧠 Grading Engine & Tolerances

The grading script evaluates user responses against multiple stored correct patterns for every item:

1. **Case-Insensitive Matching**: Automatically strips trailing whitespace and converts all user entries to uppercase.
2. **Plural & Grammatical Flexibility**: 
   - Accepts singular and plural forms (e.g., `CONDUCTOR` $\leftrightarrow$ `CONDUCTORS`, `VOLT` $\leftrightarrow$ `VOLTS`).
3. **Numeric & Scientific Unit Variants**:
   - Numbers accept raw values, values with standard units, or values with full unit names (e.g., `0.5`, `0.5A`, `0.5 AMPERES`, `0.5 AMPS`).
4. **Synonym & Acronym Recognition**:
   - Accepts both technical abbreviations and full nomenclature (e.g., `EMR` $\leftrightarrow$ `ELECTROMECHANICAL RELAY`, `ARC FLASH` $\leftrightarrow$ `FLASHOVER EVENT`).
5. **Formula Permutations**:
   - Mathematical expressions accept multiplication symbols (`*`, `X`, `·`) and spacing variations (e.g., `V=I*R` $\leftrightarrow$ `V = I X R`).

---

## 🛠️ Tech Stack

- **HTML5**: Standard semantic document structure.
- **CSS3 / Tailwind CSS (v3 CDN)**: Responsive utility-first styling with modern flexbox and grid layouts.
- **JavaScript (Vanilla ES6+)**: Client-side single-page app logic, timer routines, state synchronization, local storage handling, and regex matching routines.
- **Google Fonts (Inter / JetBrains Mono)**: Optimized typography for high legibility during study sessions.

---

## 🚀 Getting Started & Deployment

No build steps, node modules, or server-side databases are required.

### Local Execution
1. Clone or download the repository.
2. Open `index.html` in any web browser (Chrome, Firefox, Edge, Safari, or mobile web browsers).

### Free Cloud Deployment
You can host this application directly via static hosting platforms:
- **GitHub Pages**: Upload `index.html` to a GitHub repository and enable GitHub Pages under settings.
- **Netlify / Vercel**: Drag and drop the root folder containing `index.html`.

---

## 📖 Usage Instructions

1. **Navigation**: Use the **Previous** and **Next** buttons on the active question card, or open the **Question Map** drawer to jump to any item from 1 to 100.
2. **Flagging**: Click **Flag Item** on any question to mark it with an orange tag for secondary review.
3. **Filter View**: Filter the visible workspace by selecting **All**, **Unanswered**, or **Flagged** from the top control panel.
4. **Submitting**: Click the red **Submit Exam** button in the header or at the end of the question set. Confirm submission to view your score breakdown.
5. **Resetting**: Click **Retake Exam** on the results dashboard to clear saved answers and reset the timer.

---

## 📚 Study Guide Coverage

The test covers all topics from the *UP REVIEWER* curriculum:

- **Atomic Definitions**: Electron, Proton, Neutron, Nucleus, Ionization, Valence Shell, Valence Electron, Energy Levels.
- **Material Classification**: Conductors (1–3 $e^-$), Semiconductors (4 $e^-$), Insulators (5–8 $e^-$).
- **Current & Flow**: Static vs. Dynamic Electricity, Direct Current (DC) vs. Alternating Current (AC), Electron Flow ($-$ to $+$), Conventional Flow ($+$ to $-$), $360^\circ$ AC Cycles.
- **Safety & Hazards**: Electric Shock, Burns, Arc Flash / Flashover ($19,400^\circ\text{C}$ vs. Sun's $5,500^\circ\text{C}$), Body Resistance Variables (Moisture, Skin Damage, Contact Area).
- **Multimeter Operations**: Scale, Pointer, Mirror (Parallax Error mitigation), Zero Position Adjuster, Zero-Ohm Adjuster, Test Leads/Pins, Range Selector, Measuring V/I/R on live vs. de-energized circuits.
- **Circuit Testing Flowcharts**: Non-Active (Simple & Conditional Continuity, Load Resistance) vs. Active Tests (AC/DC Voltage, Current).
- **20 Electronic Devices**: Banana Jacks, Indicator Lamps (Red, Yellow/Amber, Green), Incandescent Bulbs, Bulb Sockets, Fuses & Filaments, Push Buttons (Momentary NO/NC, Emergency Mushroom Head), Terminal Blocks, Fluorescent Ballasts, Relays, Magnetic Contactors, Circuit Breakers, Overload Relays, Timers, VOM Multimeters, 9V & 1.5V Batteries, Fixed Resistors, Variable Transformers, Outlets, Variable Power Supplies.
