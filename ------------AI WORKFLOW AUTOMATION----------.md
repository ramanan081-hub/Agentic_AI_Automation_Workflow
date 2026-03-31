**------------AI WORKFLOW AUTOMATION----------n8n--------------------**

**Schedule trigger**

|---------Trigger Interval: days

|---------Days Between Triggers: 1

|---------Trigger at Hour: 10AM

|

**HTTP Request4 (6 HTTP)**

|---------Method: GET

|---------URL: http://example.com/index.html

|

**Merge**

|---------Mode: Append

|---------Number of Inputs: 6

|

**Code in Python**

|---------Mode: Run Once for All Items

|---------Language: Python

|

**AI Agent---Sub Model**

|          | 

|          |

|          **Chat Model**

|          |------Credential: Google Gemini(PaLM) Api account

|          |------Model: models/gemini-flash-lite-latest

|          |

|          **Simple Memory**

|          |------Session ID: Define below

|	   |------Key: send

|	   |------Context Window Length: 5

|

|

|

|---------Source for Prompt (User Message): Define below

|---------Prompt (User Message): MY PROMPT FOR DAILY NEWS

|

**Edit Fields**

|

|--------Mode: JSON

|--------JSON: JSON FORMAT

|

**Send a message**

|-------Credential: Gmail account

|-------Resource: Message

|-------Operation: Send

|-------To: ramanan0000@gmail.com

|-------Subject: {{ $json.subject }}

|-------Email Type: HTML

|-------Message: {{ $json.message }}

\---------------------------------------------------------------------------------

&#x20;         

