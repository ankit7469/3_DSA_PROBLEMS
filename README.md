# 3_DSA_PROBLEMS

----------------------------------------------------------------------------
##  1. Problem – ACM Team
---------------------------------------------------------------------------

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

-----------------------------------------------------------------------------------------------------
## 2. Problem - Organizing Container of Balls
-----------------------------------------------------------------------------------------------------

🎯 Purpose
- To determine whether it is possible to reorganize balls in containers such that:
- Each container holds balls of only one type.
- Swapping between containers is allowed.

🔑 Key Insight

- Each value in the matrix represents:
- matrix[i][j] → number of balls of type j in container i.
  Two important fixed quantities exist:

- Container Capacity (Row Sum)
- Total balls in each container.
- Ball Type Total (Column Sum)
- Total balls of each type across all containers.
- Since we can only swap balls (not create or destroy them):
- Container totals cannot change.
- Ball type totals cannot change.
- Reorganization is possible only if the multiset of container capacities equals the multiset of ball type totals.

🧠 Concept (Simple Explanation)
- Calculate the sum of each row → total balls in each container.
- Calculate the sum of each column → total balls of each type.
- Sort both lists.
 Compare them.
- If equal → Possible
- Otherwise → Impossible
- Order does not matter, only values matter.

🧩 Core Concepts

- 2D matrix traversal
- Row-wise summation
- Column-wise summation
- Sorting before comparison
- Multiset equality check
- Invariant preservation (totals remain fixed)

🚀 Learning Outcome

- After solving this problem, you will:
- Understand how matrix data represents structured information
- Learn difference between row-based and column-based aggregation
- Recognize invariant properties in swapping problems
- Apply sorting to compare unordered collections
- Strengthen logical reasoning for transformation-based problems

-----------------------------------------------------------------------------------------

