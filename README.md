# 3_DSA_PROBLEMS

---------------------------------------------------------------------------
##  Problem – ACM Team
----------------------------------------------------------------------------

🎯 Purpose

- To determine:

- The maximum number of topics a 2-person team can collectively know.
- The number of teams that can achieve that maximum.

🔑 Key Insight

- Each attendee’s knowledge is represented as a binary string:
'1' → topic is known
'0' → topic is not known
- When two people form a team:
- A topic is considered known if at least one of them knows it.
- This is equivalent to performing a position-wise logical OR operation.

🧠 Concept (Simple Explanation)

- Form every possible pair of two attendees.
For each pair:
- Compare their binary strings position by position.
- Count how many positions contain at least one '1'.

Track:

- The highest topic count found.
- How many teams achieve that count.

Return both values.
- No need to simulate complex operations — just compare characters.

🧩 Core Concepts

- Nested loops (pair generation)
- String indexing
- Logical OR condition
- Counting occurrences
- Maximum tracking
- Avoiding duplicate pairs

🚀 Learning Outcome

- After solving this problem, you will:
- Understand pair-based comparison logic
- Practice working with binary strings
- Learn how to track maximum values efficiently
- Improve nested loop reasoning
- Strengthen problem-solving skills for competitive programming

-------------------------------------------------------------------------------------------------------

