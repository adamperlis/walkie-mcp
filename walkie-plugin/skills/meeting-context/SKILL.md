---
name: meeting-context
description: Look up what was said or decided in Walkie meetings. Use when someone asks about a past discussion, needs action items, or wants a meeting quoted back.
---

# Meeting context

Walkie records meetings on the user's computer and exposes them over MCP as three **read-only** tools: `search_meetings`, `get_meeting`, and `list_meetings`.

## When to use

- The user asks what was discussed, decided, or assigned in a meeting
- They ask about a person, project, or phrase *in the context of* a call or discussion
- They want notes, action items, or a speaker-labeled quote

## Instructions

1. Prefer `search_meetings` with the user's keywords before asking them to name a meeting.
2. Call `get_meeting` on the best match to pull notes, action items, participants, and transcript.
3. Quote speakers and dates from the tool result — do not invent attendees or decisions.
4. If nothing matches, say so. Do not fall back to guessing from chat memory.

## Do not search unprompted

Search only when the user asks about a meeting, or asks something that plainly
can only be answered from one. Do not search on your own initiative — not while
implementing a feature that might have been discussed on a call, not to check
whether a decision exists, and not to gather background before answering.

Meeting recordings hold salary talk, reviews, interviews, and medical leave.
Pulling that into an unrelated coding session is a privacy failure even when the
transcript is the user's own, because they did not choose to open it here. When
meeting context seems relevant but was not requested, ask first: "Want me to
check your Walkie meetings for that?"
