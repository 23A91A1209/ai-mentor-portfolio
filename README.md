# ai-mentor-portfolio


# AI Mentor Bootcamp — Chilakapati Mounika

Public portfolio of 12-day AI Trainer Workshop. By Day 12: 6 daily notebooks + capstone Streamlit URL.


## Day 1 — Setup complete

- ✅ Google AI Studio API key provisioned
- ✅ Groq API key provisioned
- ✅ Hello-Gemini call working — see [Day1_Setup.ipynb](Day1_Setup.ipynb)
- 4-tool comparison matrix from Lab 1A: see screenshot below

![Gemini first call](gemini_first_call.png)


 ## Day 2 Lab 2B — Errors handled

1. **Markdown fence wrapping** (` ```json ... ``` `)  
   Gemini sometimes wraps JSON in markdown fences.  
   Retry logic forces raw JSON output, which fixes this in most cases.

2. **Missing phone number**  
   Some résumés do not include a phone number.  
   Using `Optional[str] = None` allows Pydantic to accept `null` instead of failing validation.

3. **Empty or whitespace-only input**  
   When input text is empty, Gemini cannot extract required fields.  
   Pydantic raises a `ValidationError`, which is caught and handled gracefully by the caller.

## Sample résumés processed: 3 / 3 successful

## Day 4 — n8n Daily News Digest

- ✅ Self-hosted n8n via Docker
- ✅ Workflow: Schedule (7AM IST) → RSS → Gemini summariser → Gmail
- ✅ Workflow JSON committed: [Day4_NewsDigest.json](Day4_NewsDigest.json)
- ✅ Test email screenshot below

![Test email screenshot](daily_digest_test_email.png)
