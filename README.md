# Hybrid Spam Filter

This project is an interactive, web-based spam filter that demonstrates a powerful hybrid analysis technique. It combines the speed and efficiency of a **Deterministic Finite Automaton (DFA)** for keyword-based scoring with the contextual intelligence of **Google's Gemini AI** for a deep, semantic analysis.

This application is the practical implementation of the concepts discussed in the research paper, "Design and Analysis of a Spam & Email Filter Using Finite Automata."

> **Note:** You can take a screenshot of your application and upload it to a service like Imgur to generate a URL to place an image here.

---

## Features

- **Hybrid Analysis:** Merges a fast, rule-based DFA scan with a powerful, contextual AI scan to provide a single, definitive verdict.
- **DFA Heuristic Scoring:** Uses a custom-built Deterministic Finite Automaton to detect weighted keywords and calculate a rule-based spam score.
- **AI-Powered Deep Scan:** Integrates with the Gemini AI to analyze the text for psychological tactics, suspicious intent, and other nuances that keyword matching can't catch.
- **Weighted Final Verdict:** Calculates a final score by combining the DFA result (40% weight) and the AI result (60% weight) to determine if a message is `Safe` or `Spam`.
- **Fully Interactive UI:** Add, remove, and assign risk levels (Low, Medium, High) to keywords on the fly. The DFA rebuilds instantly with every change.
- **Dynamic Visualization:** Features a stunning, animated UI with a "Matrix" theme to visualize the filtering process.

---

## Tech Stack

| Category     | Technology                                           |
|--------------|------------------------------------------------------|
| **Frontend** | HTML5, CSS3, JavaScript (ES6+)                       |
| **Styling** | Tailwind CSS                                         |
| **AI** | Google Gemini API                                    |
| **Core Logic** | Custom-built Deterministic Finite Automaton (DFA) |

---

## Setup and Installation

This project is designed to be incredibly simple to run as it is contained within a single file.

### Prerequisites

- A modern web browser (e.g., Chrome, Firefox, Safari).
- A Google Gemini API key. You can obtain one from [Google AI Studio](https://aistudio.google.com/app/apikey).

### Running the Application

1.  **Clone the repository or download the files:**
    ```bash
    https://github.com/gsaianimesh/Email-Spam-Filter.git
    ```
    Or simply download `spam_filter_app.html` and this `README.md`.

2.  **Add Your API Key:**
    Open the `spam_filter_app.html` file in a text editor. Find the following line (around line 430):
    ```javascript
    const GEMINI_API_KEY = "AIzaSyCiNcijCfp-z76WakfXg61wORMg_FPjnqo"; 
    ```
    Replace the key with your own Gemini API key.

3.  **Open in Browser:**
    Save the file and open `spam_filter_app.html` directly in your web browser. The application is now ready to use.

How to Use
Enter Text: Paste the text you want to analyze into the text box on the left.

Run Analysis: Click the "Run Hybrid Analysis" button.

View Results:

The panel on the right will instantly update.

You will see the DFA Score, the AI Confidence score, and the Final Verdict.

The "Keyword Analysis" box will show your preprocessed text with any detected keywords highlighted.

The "AI Analysis" box will show the detailed, contextual explanation from the Gemini model.

Manage Keywords: Add or remove keywords and their risk levels on the left-hand panel to customize the DFA's behavior.

Author
Ganta Sai Animesh Reddy

This project was created as a practical application for the Theory of Computation course.
