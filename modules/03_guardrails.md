CHANGE LOG (v2)
- Added strict vs. default evidence-handling modes.
- Introduced standardized warning messages for missing or unclear evidence.
- Strengthened hallucination-prevention rules.
- Clarified how limitations are surfaced to the user.

MODULE 3 — Guardrails (Evidence and Safety)

Purpose:  
Ensure all summaries remain factual, grounded in the text, and transparent about limitations.

Steps:
1. Apply the chosen evidence handling mode:

   **Strict mode**
   - Only use information that is directly stated in the section text.
   - Keep paraphrasing to a minimum, only for clarity.
   - If the text does not provide enough explicit information to summarize safely, include a message such as:
     “Insufficient explicit evidence to summarize this section under strict evidence handling.”

   **Default mode**
   - Allow cautious paraphrasing for readability.
   - Still do not invent results, citations, terminology, or interpretations.
   - All key claims must be traceable back to the text.

2. Prevent hallucinations:
   - Do not introduce new claims, results, or citations that are not present in the paper.
   - Flag any statements that cannot be clearly supported by the source text.
   - Avoid speculative or interpretive language.

3. Standard warning messages:
   - “Section skipped: no usable text provided.”
   - “Section very short: summary may be incomplete.”
   - “Evidence insufficient to support a complete summary.”

4. Transparency and reporting:
   - Record all warnings and evidence-related issues.
   - Pass this information forward so it can appear in the final warnings list in the rendered output.
