# UX Testing Reflection

## Memorability in UX (UADY Project)

### What is Memorability and where does it come from?
Memorability is that "magic quality" of an app or system that allows you to remember how to use it quickly, even if you haven’t touched it for weeks or months. You don’t have to start from scratch every time; you just pick up where you left off. This was defined by **Jakob Nielsen in 1993** in his book *Usability Engineering* as one of the five pillars of usability. He argued that a good interface must be easy to remember for users who don’t use it every day—like someone visiting a website once a month. Without this, every return feels like learning a new language.

### How it connects to the UADY project
In the UADY Medical Service, think of workers like Don José from maintenance or cleaning: they don’t book appointments daily. He might use the app today, but might not return for three or six months because his son got sick. If the interface isn't memorable, he’ll get frustrated thinking, "I don’t remember how to do this!", leading to cognitive fatigue and abandonment. He’ll end up preferring lines or phone calls, sabotaging the entire digital effort. Here, memorability is the bridge that turns the app into a habit rather than an occasional headache.

### The key metric to measure it
To move beyond assumptions, we use the **"Re-learning Rate"** (or Proficiency Recovery). This is the time it takes the user to complete a task the second time (after at least four weeks of inactivity) compared to the first. The simple formula is: **Time in Attempt 2 minus Time in Attempt 1**. If the result is close to zero or negative (faster!), it means they remembered everything well. It’s like checking if your bike still pedals smoothly after sitting in the garage for a long time.

### Real-world testing scenarios and tasks
Picture this: "Three months have passed since your last appointment. Today, your son is unwell, and you need to book a Pediatrics appointment for the morning shift next week." The tasks are concrete: open the app (with an active session), go to the scheduling module, switch to the beneficiary (the son), select the doctor and time slot, and confirm. Tests like this simulate Don José’s real life, seeing if he flows through the process without stumbling.

### What data we collect and how we analyze it
We collect hard numbers: time per task in seconds, errors (like wrong clicks that didn't happen before), and help-seeking behavior (how many times they ask "How was it again?" or look for tutorials). We also observe "soft" data: hesitations with a hovering finger, or comments like "Oh, I remember now!" versus "I can't find it." We analyze by comparing the first test (learning) with this one (memorability), like an A/B test over time. If errors are repeated, the app fails at being intuitive; it needs more "visual cues," like icons that invite interaction.

### Why it’s worth measuring in this project
It is crucial because UADY’s digital success depends on long-term use, not just the initial excitement. It prevents the **"First-Use Effect"**: apps that seem great with a guide but are forgotten on their own. For adults aged 45-55 like Don José, it provides autonomy and confidence—no more asking their kids for help every time, which boosts satisfaction. Administratively, it reduces support calls, errors like duplicate appointments, and system chaos. Ultimately, memorability transforms the app into a reliable ally.


### References
*   Nielsen, J. (1993). *Usability Engineering*. Morgan Kaufmann. (The foundation for the definition of memorability).
*   Nielsen Norman Group: "Usability 101: Introduction to Usability" ([nngroup.com](http://nngroup.com)). Discusses occasional users and abandonment due to lack of memorability.