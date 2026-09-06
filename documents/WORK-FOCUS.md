# How I Work – Quality & Stability focus

A broad baseline about beliefs and guidelines for general software development.
I'd apply these for commercial work and projects – given there are no existing definitions or requirements yet.

## TOC

- [Business side](#business-side)
- [Growing demands](#growing-demands)
- [Footnotes](#footnotes)

<br>

---

<br>

## Business side

1. Problem first, solution second: Goals and needs shall drive innovation
2. Simplicity: Avoid anything without measurable value. If no measure exists, research and make a best assumption - check later.
   - Keep costs, dependencies, and risks low. Craft minimal solutions – not just for humans, but also for AI tooling. Reduce confusion or
     undesired 'inspiration', e.g., from leftover/ legacy remainders.
3. Longevity vs. realism: Build for the future, but not forever. Be realistic about software lifecycles, dependencies, and maintenance costs.
   - Don't build the perfect system; have it working now; expand and refactor later.
4. Critical thinking and oversight: Don't assume and blindly believe; test and prove.
   - Combine deterministic and probabilistic approaches. Apply human judgment and skill.
5. Compatibility with the latest devices (unless there are specific needs):
   - Build for the ~98th percentile. Check if the remainder truly matters and what impact optimizations have.
   - Focus on the rest, when it's measurable. Consider the cost of development, and maintenance vs. a potentially beneficial CR.
   - Consider accessibility and usability at least for the legal minimum.
6. Don't rely on certain vendors - Always abstract their use, in case of future changes.
   - Always have another potential option at hand, that would be fast to integrate and switch to. TOS, pricing, leadership, and reliability changes.

## Growing demands

1. Simple code, not to impress any idols:
   - Follow industry standards and stick to these.
   - Code must speak for itself. Clean, practical types, no type juggling with many layers of abstractions.
   - Consistent abstractions and architecture - for human teams and AI getting inspired by any of it.
   - Simple abstractions, no over-architecting. A code file with 500 lines is perfectly fine if it has a single layer of complexity (e.g., HTML or data structures).
     Abstract complexity by logic and demand, not for the line count or other measures.
     - A single file to search and edit a single cohesive, logical unit of information is easier to understand,
       and ultimately faster and cheaper to work with than looking through file system imports and abstractions.
2. Quality from the core, but do not overdo it: Introduce suitable tooling and pipelines once, or consider gradual adoption and refactoring demands. The better the foundation, the fewer delays, rework, risks, and bugs that disrupt the business model later.
   - Apply solid engineering, code analysis, linting, and formatting - But don't enforce it for every single change (e.g., commit hooks that drain performance). Avoid slowing down development, but make it mandatory before it's released.
   - Be realistic about last-minute emergency fixes, and don't block this path if ever needed.
   - Don't beautify to satisfy 'best practices' if it affects the whole team and hundreds of files.
     Leave it out, or consider a one-shot adoption in a risk-free period without ever sacrificing application stability.
   - Be strict about code integrations – No 'admin' or lead approvals to bypass rules shall occur.
   - Slow and complex tools might run at different cycles and be isolated from day-to-day workflows;
3. Test critical paths, not everything – e.g., just for a '100%' score or coverage,
   the cost of creation and maintenance can outweigh any benefit.
   - e.g., E2E or live tests/ scraping can be slow, expensive, and fragile. Use for vital parts.
   - A good-looking component doesn't guarantee a feature is functioning.
4. Integrate logging and tracking: Review what happens on the real system, with real users and data.
   Define and track KPIs and watch out for unusual patterns or errors.
5. Secure by default: Least privilege, no secrets or PII, no hardcoded passwords.
   - Craft a workable, practical baseline from the start – This one is easy to fail in stressful times and environments, as it can be easily bypassed or ignored.
   - Containerize and isolate environments; forbid local use. Delay package introduction for the benefit of vulnerability fixes. Pin versions.
   - Consider AI implementations as helpful but not secure by default. Double-check if all rules and best practices are followed and introduced measures are up-to-date.
   - Care about what you can and should do, responsibly, and hire an expert to audit when required.
6. Replace legacy stacks with stable newcomers, e.g., for utility tooling
   - If the ecosystem is mature enough to do so and benefits outweigh costs
   - Assure consistency across internal teams and external contributors

<br>

---

<br>

## Footnotes

Many of these topics are simple and cost-efficient to mitigate, and can provide benefits from day one.
Given, the business priorities give space to quality engineering, and teams have a common standard to work towards.

I've often seen this as a missed opportunity, where application quality and security receive limited attention, even in larger organizations.
In the beginning, the impact can be difficult to measure.

As software grows, however, more issues can accumulate. Without shared practices and standards, the teams' focus shifts to firefighting mode instead of innovation.
Quality does not necessarily increase with experience. It benefits from standardization and automation.

_Consider something as simple as a typo: in the wrong place, it can break an application, cause a failed deployment, and leave the entire team waiting for a fix._

Learning from mistakes is one thing – preventing avoidable ones saves time and resources.

### Optimistic words …

The goal is not a perfect, error-free environment – but a predictable, reliable one.

Your team knows how it works. The newbie can learn it in half a day. If it ever fails, it's too rare to be agitated by it and easier to solve.
Deployments on Friday evening might even become a staple, with everyone looking forward to a wonderful Monday and empty postboxes without complaints or error reports.

Resilience goes beyond the code itself.

<br>

---

<br>

_Some of these statements are likely subjective. Enterprise systems might need more and stricter rules. Small and fast ventures, much less._
_I don't see these as universal truths. The ultimate goals are a common understanding and reliability – any contribution is welcome. Technology evolves; so should we._
