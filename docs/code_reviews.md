# Code Reviews

**Purpose:**
    - To define what code reviews are.
    - Why they're important for everyone.
    - To give practical and functional guidelines for both reviewers and authors.

**Goal:**
    - To improve code quality.
    - To increase the knowledge on Code reviewers.
    - Promote a more positive collaborative culture.

-- 

## 1. Overview & Benefits

**What are code reviews?**
- Code reviews is a process that examines any code changes that are made before merging into the main branch.
- It focus on improving the quality of the code, catching any problems early and sharing experience with your team.

**Key Benefits:**
- Enhanced Quality: This helps identify bugs, improve the codes readability and ensure consistency.
- Collaboration: Creates a mutual learning and shared code ownership.
- Issue detection: Allows the team to catch any defects before they send a product out for production for example.

    ```mermaid
    graph TD;
        A[Developer Submits Pull Request] -->|Automated Tests Run| B{Tests Pass?};
        B -- No --> C[Fix Issues and Resubmit];
        B -- Yes --> D[Peer Code Review];
        D -->|Review Passed?| E{Approved?};
        E -- No --> F[Provide Feedback & Request Changes];
        F --> A;
        E -- Yes --> G[Merge to Main Branch];
        G --> H[Deployment & Monitoring];
        
        subgraph Benefits of Code Reviews
            I[Improves Code Quality] 
            J[Encourages Collaboration]
            K[Detects Issues Early]
            L[Ensures Consistency]
            M[Knowledge Sharing]
        end

        G -->|Code is Merged| I & J & K & L & M;

--

## 2. Best Practices for Reviewers
The aim for this is to provide a clear guideline for any team to ensure constructive and efficient reviews.

**Delivery & Feedback:**
    - Be respectful and focus on only the code not the person coding. 
    - Make sure the questions being asked are precise and clarifying to read and understand.

**Guidelines:**
    - Point out the exact area that are needed for improvement.
    - Explain why they need to make the change.
    - Give effective solutions and clean code.

**Reviewers Checklist:**
    - Is the code clear and understandable?
    - Are the tests comprehensible?
    - Does the code follow the standard set?
    - Are there any issues with security or performance?

--

## 3. Best Practices for Code Authors
The aim for Authors is to equip them with pratical steps to prepare their code for a steady review process.

**Preparation**
    - Reviewing own work for any issues before submitting.
    - Reduce the size of large features into smaller pull requests.
    - Add detailed descriptions and contexts about the pull request.

**Engagement**
    - Be open to feedback and ask questions.
    - Update any relevant documentation and tests as needed.

**Do's**
    - Write a clear commit message.
    - Update relevant documentation.

**Dont's**
    - Submit huge changes that have no aim.

--

## 4. Tools and Automation

---

## 5. Common Pitfalls & Mitigation Strategies

---

## 6. Quick Reference Summary

---

## 7. Conclusion & Next Steps

---

## 8. References

---

1. **[How to Make Good Code Reviews Better](https://stackoverflow.blog/2019/09/30/how-to-make-good-code-reviews-better/)** – Stack Overflow Blog (2019)

2. **[Code Review Best Practices. How to make people like your code review?](https://tsh.io/blog/code-review-best-practices/#:~:text=Reviewing%20the%20code%20means%20one,personal%20code%20review%20best%20practices)** – Marcin Gajda (The Software House blog, 2020)

3. **[Code Review Guidelines for Humans](https://phauer.com/2018/code-review-guidelines/#:~:text=Code%20reviews%20are%20powerful%20means,effective%20and%20respectful%20code%20review)** – Philipp Hauer’s Blog (2022)

4. **[Code Review Best Practices](https://blog.palantir.com/code-review-best-practices-19e02780015f?gi=2c7d3ff9542a#:~:text=,adds%20implementations%20for%20those%20interfaces)** – Palantir Engineering Blog (2018)

5. **[5 Best Practices for Code Reviews](https://www.codelantis.com/blog/code-reviews-best-practices)** – Codelantis Blog (2023)
