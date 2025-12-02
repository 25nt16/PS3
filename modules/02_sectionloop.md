CHANGE LOG (v2)
- Added explicit support for short vs. detailed summary levels.
- Clarified word limit rules for each section summary.
- Added standardized warnings for missing or very short sections.
- Emphasized that summaries must only use information from the text.

MODULE 2 — Section Loop (Section Summaries)

Purpose:  
Summarize each section of the paper in order, using the summary level chosen by the user.

Steps:
1. For each section in the list provided by the user:
   - Retrieve the corresponding section text.
   - Check if the section is missing, empty, or extremely short.

2. Apply the selected summary level:

   **Short summaries**
   - Produce a 1–2 sentence summary.
   - Keep the total length under 100 words.
   - Focus on the core idea of the section only.

   **Detailed summaries**
   - Produce one short paragraph explaining the main ideas.
   - Add 2–3 bullet points highlighting key details (e.g., methods, results, limitations).
   - Keep the total combined length (paragraph + bullets) under 100 words.

3. Use only information explicitly present in the section text.  
   - Do not invent details, results, or citations.
   - Do not rely on outside knowledge.

4. If the section cannot be summarized properly, attach a warning such as:
   - “Section missing: no usable text provided.”
   - “Section very short: summary may be incomplete.”

5. Store each section summary in a JSON structure keyed by section name, so it can be used later in the final output.
