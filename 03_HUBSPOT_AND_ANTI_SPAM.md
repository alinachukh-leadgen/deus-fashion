# DEUS ROBOTICS — HUBSPOT ACTIVITY & ANTI-SPAM PROTOCOL

## Objective

Claude has access to HubSpot and must use it as the source of truth for outbound activity.

The purpose is to prevent:
- duplicate outreach;
- channel collisions;
- repeated pitches;
- contacting someone too frequently;
- losing the context of previous conversations.

---

# 1. PRE-SEND CHECK — MANDATORY

Before ANY outbound email or LinkedIn message:

### Step 1 — Find the contact
Confirm:
- correct person;
- correct company;
- role;
- email/LinkedIn identity.

### Step 2 — Open the company/contact activity
Review:
- outbound emails;
- inbound replies;
- LinkedIn messages if available;
- meetings;
- notes;
- tasks;
- previous sequences/campaign activity.

### Step 3 — Calculate the last outbound touch

Identify the most recent outbound:
- email;
- LinkedIn DM;
- connection request if logged;
- other direct outreach.

### Step 4 — Apply 14-day rule

If less than 14 days have passed:
STOP.

Do not send another direct message.

If exactly 14 days or more have passed:
continue, provided there is a legitimate reason for the new touch.

### Step 5 — Check content overlap

Ask:
- Have we already used this trigger?
- Have we already asked this question?
- Have we already made this claim?
- Did they ignore, answer, decline, or ask for timing?
- Is there a new reason to contact them?

---

# 2. WHAT COUNTS AS SPAM

For this workflow, spam means sending a direct outbound message more frequently than once every two weeks.

This is a strict operational definition for Claude's workflow.

The rule is channel-agnostic.

Examples:

Email on Oct 1
→ LinkedIn DM on Oct 8 = NOT allowed.

LinkedIn DM on Oct 1
→ Email on Oct 15 = allowed only if there is a valid reason and the minimum interval has elapsed.

Email on Oct 1
→ email Oct 15 = allowed.

---

# 3. SAME-DAY LOGGING

Every outbound action must be logged in HubSpot on the same day.

At minimum record:
- date;
- channel;
- direction;
- contact;
- company;
- short message summary;
- trigger;
- CTA;
- outcome if known;
- next action/date if relevant.

Do not move a deal stage simply because outreach occurred.

---

# 4. IF THERE IS A REPLY

Stop automated outbound.

Read the response.

If they:
- ask a question → answer it;
- show interest → move toward a meeting;
- ask to follow up later → log the requested date and honor it;
- decline → respect the decline;
- redirect to another person → update the contact path.

Do not continue a generic sequence after a meaningful reply.

---

# 5. IF A MEETING IS BOOKED

Log:
- meeting date;
- participants;
- source of meeting;
- converting message;
- trigger;
- key interest;
- expected next step.

The message that converts is a valuable sales asset. Preserve it as a proven example.

---

# 6. IF THERE IS NO RESPONSE

After 14 days, ask:
"Do I have a new reason to write?"

If no:
wait.

If yes:
write a new message around the new reason.

Do not create artificial reasons merely to satisfy cadence.

---

# 7. HUBSPOT DATA QUALITY

Claude should avoid creating:
- duplicate contacts;
- duplicate companies;
- duplicate activities;
- contradictory notes.

If the same activity appears in multiple places, use the most authoritative record and do not double-log it.

---

# 8. IMPORTANT CHANGE FROM THE OLD PLAYBOOK

The old playbook explicitly recommends logging every step in HubSpot the same day.

That remains mandatory.

The old outreach cadence was four emails over roughly three weeks.

That cadence is no longer the governing cadence.

The current rule is:
MINIMUM 14 DAYS BETWEEN DIRECT OUTBOUND TOUCHES.
