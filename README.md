# Minor_Project_1

GroupDNA — Your WhatsApp Group Chat, Decoded
"Spotify Wrapped, but for your friend group."

GroupDNA is a behavioral data analytics tool written completely from scratch. It parses a raw, plain-text WhatsApp chat export file, handles real-world formatting inconsistencies, and produces an executive visual dashboard tracking conversational velocity, hourly rhythms, slang dictionaries, response behaviors, and custom personality archetypes.

📸 Dashboard Output Preview
The engine renders a high-fidelity terminal dashboard using printable block characters and strict column alignments: 
Refer to the following execution states for full text-art visual context:
Screenshot 2026-06-29 155741.png
Screenshot 2026-06-29 155758.png

🛠️ Project Design & Constraints
This project is deliberately engineered around algorithmic restraint and constraint discipline. To showcase proficiency with mathematical logic and optimization primitives, the use of automated wrapper libraries was completely banned

🚫 STRICTLY FORBIDDEN:
No Pandas (No DataFrames, no read_csv)
No Data-Viz Modules (No Matplotlib, Seaborn, Plotly)
No Regular Expressions (No re imports)
No Pre-built Collections (No Counter, defaultdict)

✅ ALLOWED & UTILIZED
Pure Python data primitives (lists, dicts, tuples, sets)
NumPy Primitives (np.zeros, array masking, indexing, row/col reduction)
Pure String Manipulation (.split(), .strip(), .isupper(), .replace())  
Native datetime parsing (datetime.strptime, timedelta)

🚀 Core Architectural Features
1. Robust Chat Parsing Engine
- Reads raw WhatsApp logs line-by-line using basic file I/O operations and tokenizes structural components safely while accommodating critical edge cases
- System Alerts: Traps notifications (e.g., encryption warnings, group modifications) without breaking index counts.  
- Media / Deleted Messages: Isolates flags like <Media omitted> and This message was deleted to compute sharing frequencies separate from raw token lists.  
- Multi-line Continuation: Dynamically captures single text blasts separated by hard carriage breaks using structural date anchor checkpoints.  

2. Time-Series Activity Heatmapping
Maps conversational volume distribution by binding spatial coordinate elements into a 6×24 NumPy Matrix. Row indices track individual users across columns indexing 24-hour time arrays. The data normalize user-relative volumes to yield dynamic density scales rendered directly to the terminal workspace (., ░, ▒, █).  

3. Native Text-Mining & Stopword Interception
- Punctuation blocks are programmatically stripped via linear string modifications. Texts are tokenized and processed against an isolated vocabulary checklist of common English and Hindi filler words, isolating authentic inside jargon and calculating visual frequency distributions.

4. Dynamic Personality Archetype Matrix
- Assigns a distinct personality classification to each user using quantified behavioral conditions:
      - 💬 THE SPAMMER: Highest continuous back-to-back messaging blocks without active structural conversation context switches.
      - 🦉 THE NIGHT OWL: Concentrates >60% of total output volume explicitly within late-night/early-morning constraints ($23:00 - 04:59$)
      - 📖 THE STORYTELLER: Tallies extreme text lengths, maintaining high descriptive average word boundaries per single transmission.
      - 👑 THE DRAMA QUEEN: Tracks high uppercase distributions and heavy punctuation anomalies (e.g., consecutive ! characters).
      - 👻 THE GHOST: Computes long historical dry spells, finding users with long consecutive silent streaks over active group timeline spans.
      - 👔 THE PAKKA PUNCTUAL (Custom Invented Archetype): Automatically flags group members executing communication patterns restricted to sensible corporate                 hours ($09:00 - 18:00$), identifying organized off-screen balance.
  
📊 Dataset Profile & Verification Results
Tested against the official synthetic hostel_bois.txt tracking 6 concurrent participants across a locked 60-day window:
- Total Clean Messages Processed: 3,174
- Busiest Window: 04 May 2024 (76 messages mapped)
- Timeline Range: 01 April 2024 to 30 May 2024

📦 How To Run
- Export any chosen WhatsApp conversation chat history as a .txt file (choose Without Media inside the application export panel)
- Name your file hostel_bois.txt or change the FILE_NAME declaration inside your environment file pointer.
- Run the notebook sections sequentially from top to bottom

🎓 Acknowledgments
- Deep gratitude to Girish Sir and the technical coordinators at The Unlox Academy for designing this project constraints matrix. Stripping standard libraries away built solid engineering discipline and structural algorithmic clarity.

Developed by Mohit Patel | Built with Python + NumPy Primitives 🐍

 
