# Command: /scrape-competitors

## Description
Triggers the SEO workflow in n8n.

## Instructions

When this command is executed:

1. Send a POST request to:
https://cxlinstitute.app.n8n.cloud/webhook/scrape-competitors

2. Use the following JSON payload:

{
  "trigger": "claude_code",
  "timestamp": "{{current_timestamp}}",
  "input": "{{user_input}}"
}

3. Do not perform any additional processing.
4. Do not generate SEO analysis.
5. Only act as a trigger.

## Output

If successful:
"✅ SEO workflow triggered successfully."

If failed:
Return the error response.