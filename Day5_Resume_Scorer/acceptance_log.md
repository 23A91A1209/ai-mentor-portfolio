## Day 5 Lab 5A — Continue.dev acceptance log

1. Accepted: bar_chart visualization of sub-scores
   Why: makes the score breakdown immediately scannable

2. Accepted: prompt modification adding 4 sub-fields
   Why: needed for the bar chart and keeps the prompt-output contract clear

3. Accepted: learning resources structure
   Why: provides actionable next steps for improving résumé fit

4. Accepted: learning_resources JSON field
   Why: allows structured output that Streamlit can display easily

5. Accepted: Top 3 Missing Skills & Learning Resources section
   Why: helps users identify skill gaps and find free learning materials

6. Accepted: use of result.get('learning_resources', [])
   Why: prevents errors if Gemini does not return the field