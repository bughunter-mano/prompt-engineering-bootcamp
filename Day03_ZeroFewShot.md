# Day 3 — Zero‑Shot vs Few‑Shot
**Task:** Sentiment classify 5 customer comments about a hypothetical app **StudyBuddy AI**.

## Comments
1) "The app helped me organize my studying — love it!"  
2) "It crashes sometimes. Not sure if I’ll keep it."  
3) "Exactly what I needed. Great reminders and clean design."  
4) "Too many notifications. Annoying."  
5) "Support replied fast and solved my problem. Thanks!"  


---
## A) Zero‑Shot Prompt (run first)
Classify the sentiment of each comment as **Positive / Neutral / Negative**. Return a simple table with two columns: Comment # and Sentiment.

**Your Zero‑Shot Output:*Comment #	Sentiment
1	Positive
2	Neutral
3	Positive
4	Negative
5	Positive*

---
## B) Few‑Shot Prompt (run second)
Here are labeled examples:
- Text: "I love the interface and it keeps me on track." → Positive  
- Text: "It’s okay, but I’m undecided." → Neutral  
- Text: "App keeps freezing — very frustrating." → Negative

Now classify the 5 comments above. Return the same table format.

**Your Few‑Shot Output:*Comment #	Sentiment
1	Positive
2	Negative
3	Positive
4	Negative
5	Positiv*

---
## Reflection (2–3 lines)
What improved with few‑shot examples?
The few-shot examples provided clear guidance on how to interpret ambiguous comments. For comment #2, the example of "undecided" helped me correctly classify "Not sure if I’ll keep it" as a Neutral sentiment. The zero-shot prompt's response of "Neutral" was an error.
