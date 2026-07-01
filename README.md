# Minor_Project_1

# GroupDNA: Your WhatsApp Group Chat, Decoded 🧬

> **"Spotify Wrapped, but for your friend group."**

GroupDNA is a Python-based behavioral analytics tool that transforms a raw, messy WhatsApp chat export (`.txt` file) into a beautifully formatted, visually striking personality and activity report. 

The defining highlight of this project is its strict **Constraint Discipline**—the entire pipeline is engineered **without Pandas, Matplotlib, Seaborn, or Regular Expressions (Regex)**, relying solely on Python fundamentals and a single NumPy matrix for the core logic.

---

## 📸 Project Showcase & Reference Output

The screenshots below show the final terminal-style analytics report generated inside the Google Colab environment using the synthetic dataset `hostel_bois.txt`:

### 1. Group Overview & Activity Heatmap
![Group Overview & Activity Heatmap]<img width="982" height="977" alt="Screenshot 2026-06-29 155741" src="https://github.com/user-attachments/assets/34e3684a-1616-46e4-aad1-abb69cd09058" />


### 2. Word Frequency, Response Patterns & Archetypes
![Response Patterns & Archetypes]<img width="987" height="972" alt="Screenshot 2026-06-29 155758" src="https://github.com/user-attachments/assets/33871099-315c-46de-8536-cdceb11baea9" />


*Note: Ensure these image files are uploaded directly to the root of your GitHub repository so they render correctly in this README.*

---

## 🎯 Key Features Implemented

The project successfully implements all **8 Core Mandatory Features** outlined in the `GroupDNA_Minor_Project_Brief.pdf`:

1. **The Chat Parser:** Iterates through raw lines, handling system alerts, deleted logs, multi-line entries, and media omissions (`<Media omitted>`) to extract clean data streams.
2. **Group Overview:** Displays critical headline statistics, including message distribution percentages and a sorted participant ranking[cite: 1].
3. **Busiest Day & Hour:** Identifies the precise day and collective peak hour across the entire chat duration[cite: 1].
4. **Activity Heatmap (NumPy Matrix):** Bins user message frequencies into a `6 x 24` NumPy matrix, mapped out visually using customized printable text shading blocks (`.`, `░`, `▒`, `▓`, `█`)[cite: 1].
5. **Top Words Tracker:** Tokenizes chat history, filters custom stop-words, and outputs a horizontal block-character bar graph representing vocabulary trends[cite: 1].
6. **Response Gaps & Silent Streaks:** Parses text timestamps into native Python datetime objects to determine precise average reply times and longest consecutive ghost periods per member[cite: 1].
7. **Personality Archetype System:** Runs user metadata through exclusive quantitative scoring rules to tag everyone with a definitive social archetype[cite: 1].
8. **The Final Report Layout:** Wraps all analytical engines into a singular, highly scannable output using careful f-string padding and box-drawing elements[cite: 1].

---

## 🚫 Constraints & Technical Ground Rules

To demonstrate underlying data science skills, standard abstractions were intentionally avoided[cite: 1]. The architecture maps directly to these strict boundaries:

| Allowed Features 🟢 | Forbidden Libraries 🔴 |
| :--- | :--- |
| **Python Core Elements** (Loops, Lists, Sets, Tuples, Dicts, Functions, Comprehensions)[cite: 1] | **Pandas** (No DataFrames, no `read_csv`)[cite: 1] |
| **NumPy Matrix Engine** (Array slicing, integer indexing, multidimensional shapes)[cite: 1] | **Matplotlib / Seaborn / Plotly** (Visualizations must be purely terminal-based)[cite: 1] |
| **Built-in String Methods** (`split`, `strip`, `lower`, `isupper`, etc.)[cite: 1] | **re (Regex)** (All parsing completed via standard string methods)[cite: 1] |
| **Datetime Module** (`strptime` and `timedelta` exclusively for time-math logs)[cite: 1] | **Pre-built WhatsApp Analyzers** or Heavy NLP Toolkits (No NLTK, Scikit-learn)[cite: 1] |

---

## 🧠 Quantitative Archetype Mechanics

Participants are grouped exclusively into unique archetypes by evaluating operational metrics[cite: 1]:

* **THE SPAMMER:** Triggered by high message bursts back-to-back without group interruption[cite: 1]. *Dataset result: Rahul (Avg burst 4.5)*
* **THE GROUP MOM:** Dictated by the highest frequency of empathetic and care-focused tracking keywords[cite: 1]. *Dataset result: Priya*
* **THE NIGHT OWL:** Flags members distributing over 60% of total activity late into the night (23:00 to 04:59)[cite: 1]. *Dataset result: Aman (79.8% metrics)*
* **THE STORYTELLER:** Attributed to text logs maintaining verbose message architectures (>30 average words per entry)[cite: 1]. *Dataset result: Karan (Avg 57.0 words)*
* **THE DRAMA QUEEN:** Driven by accounts with >30% text lines entirely in ALL-CAPS or packed with multiple exclamation marks[cite: 1]. *Dataset result: Neha (63.3% ALL-CAPS)*
* **THE GHOST:** Surfaces members spending more than 60% of the recorded timeline completely silent[cite: 1]. *Dataset result: Vikas (Silent on 44 out of 60 days)*

---

Represented by : Mohit Patel
