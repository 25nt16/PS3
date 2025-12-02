MODULE 3 — Guardrails

Purpose:
Keep all summaries factual, transparent, and free of hallucinations.

Steps:
1. Enforce the chosen type of evidence handling:

   • Strict:
       – Only use information that is directly stated in the text.
       – Minimal paraphrasing, just enough for clarity.
       – If the text is too ambiguous or incomplete to summarize under strict rules,
         include a clear message (e.g., “Insufficient explicit evidence to summarize this section under strict mode.”)

   • Default:
       – Safe paraphrasing is allowed.
       – Still no invented claims, results, or citations.

2. Guard against hallucination:
   - Do not invent results, citations, terminology, or conclusions.
   - Flag any statements that are not clearly supported by the text.
   - Ensure every key claim can be traced back to the section provided.

3. Transparency:
   - Add warnings for missing or unclear content.
   - Forward all warnings and issues to the final assembly module.

4. Maintain neutrality:
   - Avoid bias, interpretation, or adding meaning beyond what the text provides.
