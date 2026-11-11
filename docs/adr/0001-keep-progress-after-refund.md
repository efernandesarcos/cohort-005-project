---
status: accepted
---

# Keep a Student's progress when a Refund ends their Enrollment

When an Admin approves a Refund Request, the Student's Enrollment ends at once, but their Course Progress and Watch Time (lesson completions, quiz attempts and video watch history) are kept, not deleted. Deleting can't be undone, while keeping costs nothing: a Student with no Enrollment can't see the course anyway, and if they buy it again they carry on where they left off.

## Considered Options

- **Delete progress on approval.** Rejected: it can't be undone if an approval was a mistake, and it would change figures already reported, such as instructor analytics and the Watch Time an Admin saw when deciding.
- **Keep progress (chosen).** Progress already belongs to the Student and the lesson, not to the Enrollment, so keeping it needs no extra work.

## Consequences

- A refunded Student who buys the course again keeps their old Course Progress and Watch Time. This is only safe because a course that has been refunded once can never have another Refund Request; otherwise a Student could buy, watch a little more, get refunded, and repeat.
- A refunded Student's learning history stays in the database. If a data-deletion request comes in, it has to be handled separately; this decision does not cover it.
