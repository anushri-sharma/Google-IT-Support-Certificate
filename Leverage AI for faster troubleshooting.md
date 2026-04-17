# Leverage AI for faster troubleshooting


### 🔍 Daily reality: troubleshooting and log analysis consume significant IT time

– **Logs contain large volumes** of technical details, error codes, and jargon that make manual analysis slow.

– Slow root-cause finding increases **downtime** and reduces client productivity.

### 🤖 What Gen AI can do for troubleshooting

– **Sift massive log data** to pinpoint anomalies and errors that are hard for a human to detect.

– **Identify which logs** to review and **prioritize events** by severity and impact.

– Produce concise, easy-to-follow summaries that speed root-cause analysis.

### ✅ Concrete example: intermittent Wi‑Fi outages for a user and six colleagues

– Collected logs by having users run diagnostic commands when the issue recurred.

– Prompt used (paraphrased): “A user is experiencing intermittent connectivity issues while connected 
to Wi‑Fi. These are the details from **wdutil info.** What can this tell us about their issue?”

– **Sensitive identifiers removed** from logs before analysis.

– **Gemini** flagged a **transmission rate of 8.0 megabits per second** as too low for **Wi‑Fi 6**, 
and suggested **distance from the router** as a probable cause despite relatively strong RSSI and low noise.

### 🛠 Validation and remediation workflow used
– Validated the AI findings with independent research into transmission-rate implications.
– Requested a **heat map** from the networking team to verify coverage and AP placement.
– Confirmed users were seated in a corner with APs far away; networking team **deployed a new AP** to improve coverage.

### ✍️ Prompting and data-prep best practices
– **Include specific context: operating system, approximate time** of occurrence, and **symptoms**.
– Attach relevant logs and state which command or tool produced them (example: **wdutil info**).
– **Remove confidential or identifiable data** before sending logs to an AI tool.
– Ask targeted questions that indicate what the AI should focus on.

### ⚠️ Responsible use and verification requirements
– Treat AI output as **assistive, not definitive**; always verify with additional diagnostics or expert teams.
– Cross-check numerical findings and network hypotheses before implementing changes.
– Maintain data-privacy practices when sharing logs with AI systems.

### 💡 Practical benefits and implications for IT operations
– Faster identification of root causes leads to **reduced downtime** and **improved support**.
– AI can surface subtle indicators (e.g., mismatch between **transmission rate** and Wi‑Fi standard) that humans may miss.
– Combining AI analysis with targeted manual validation and team collaboration yields reliable fixes.

### 🔎 Limitations and edge cases to watch for
– AI may not infer physical or environmental factors without supplemental data (e.g., seating location, AP map).
– Misleading or incomplete logs can produce incorrect conclusions; additional measurements or maps may be required.
– Overreliance on AI without validation risks misdiagnosis and incorrect remediation.


#### Example Gemini Prompt:

I used Gemini to go through the logs and get a better understanding of what was going on.

I enter a prompt like this.
<img width="775" height="574" alt="image" src="https://github.com/user-attachments/assets/ee56b665-e01a-40f0-b341-43037d81134f" />

A user is experiencing intermittent connectivity issues while connected to Wi-Fi.

These are the details they get when running **wdutil info command**.

What can this tell us about their issue?

This helps Gemini know what it should focus on, which is any error that can tell us more about the connectivity issue.

Then I added the relevant part of the logs.

I copied and pasted these logs on a note and removed any identifiable information, like the customer's wifi network name.
<img width="640" height="625" alt="image" src="https://github.com/user-attachments/assets/87d27b97-d3b3-4d12-9f7a-c1d162eb610f" />


Gemini pointed out the transmission rate of 8.0 megabits per second was too low for Wi-Fi 6.

This is insightful because I might have overlooked that fact given that the RSSI signal strength was relatively strong, and there wasn't much noise interference.

Not only did it flag the transmission rate as an issue, but it also noted the distance from the router as a probable cause in its response.

I made sure to validate Gemini's analysis and conduct my own research on the transmission rate.

I also asked the networking team to generate a heat map of the area where the user and their colleagues were seated.

I discovered that they were sitting in a corner of the building with the closest Wi-Fi access points, or APs, being far away, just as Gemini had suggested.

To address the issue, the networking team deployed a new AP to improve the coverage in that area.

If you use AI to help you with troubleshooting, make sure you include specific context such as the operating system,

approximate time the issue occurred, and the symptoms of the problem, along with the logs when you write your prompt.

Don't forget to remove any confidential data from the logs, and verify the results by doing your own research on the answers provided by an AI tool.

## Communicate technical concepts with AI

### 💡 Communication challenge in IT support

– **Customer care** requires resolving issues to the user's satisfaction, which often means translating **complex technical terminology or instructions** for non-technical users.

– Users with technical problems may be **frustrated or anxious**, increasing the need for clear, empathetic instructions to prevent misunderstandings.

### 🔧 Use of Gen AI to simplify technical guidance
– **Gen AI tools** (example: **Gemini**) can **rewrite responses, change tone**, and **simplify jargon** to produce clearer guidance.
– Demonstrated case: needed a non-technical user to run **Windows network troubleshooting commands** to **reset network configurations**; the AI generated a **user-friendly, step-by-step guide** suitable for someone unfamiliar with the Command Line.

### ✅ Verification and customization requirements
– Always **verify the AI-generated response** for technical accuracy before sending.
– **Tweak the wording** to match your personal communication style or add a custom greeting to maintain professionalism and context.

### 🗣️ Adjusting tone, length, and format for the user/channel
– If the AI reply is too long for chat, prompt it to "**shorten this**" or specify the desired **format** (bullet steps, numbered list, etc.).
– Request the AI to make the response **more casual or more formal** to match the user's tone or the communication channel.

### ⚠️ Practical implications and guardrails
– Using AI can **reduce misunderstandings** and help non-technical users feel comfortable following instructions.
– Do not over-rely on the AI output; maintain oversight to ensure instructions are safe, accurate, and appropriate for the user's skill level.

### ⏱️ Productivity and client experience outcomes
– Integrating AI into daily client communication can **increase productivity** and improve clarity.
– Clear, direct communication from AI-enhanced messages can lead to **better client satisfaction** and stronger working relationships.

<img width="775" height="524" alt="image" src="https://github.com/user-attachments/assets/4656b447-f1d2-4525-b2ba-334fc443901d" />

**Output:**

<img width="1232" height="463" alt="image" src="https://github.com/user-attachments/assets/1a04ec59-9a90-44f1-84f8-a251d9aa96dc" />
<img width="1216" height="601" alt="image" src="https://github.com/user-attachments/assets/f0dd5acc-31eb-4210-95a9-27768b408e76" />
