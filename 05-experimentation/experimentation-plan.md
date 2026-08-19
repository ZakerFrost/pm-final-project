# Experimentation Plan (Module 5)

## Get your documents ready
- **From M3, your hypothesis sentence:** Based on qualitative evidence that low-intent viewers find discovery effortful and a current 29% Start Rate, I believe adding a human-curated Spotlight Rail for Wanderers and Casual Browsers will increase successful transitions from homepage discovery to playback. Success is an absolute +3 percentage-point increase in Start Rate, from 29% to at least 32%, versus Control. We will run the experiment for a minimum of 14 days and until 3,697 analyzable observations per arm are reached, while ensuring Power User weekly sessions do not decline by more than 5% where Power Users are exposed to the treatment.
- **From M3, your primary success metric & guardrail metric:** Start Rate = % of eligible Wanderer/Casual Browser homepage sessions resulting in playback starting.
They have to remain within 5% of the existing 4.8 sessions/week baseline.
- **From M4, the feature you scoped in your PRD this is what you're testing:** Spotlight Curated Rail

## Define your experiment parameters
- **Feature under test pull from your M4 PRD:** Spotlight Curated Rail
- **Persona pull your M2 persona:** A low-intent subscriber who wants easy entertainment but rarely invests effort discovering something new.
- **Expected outcome the behaviour change you expect, from your M3 hypothesis:** Increase successful discovery and new-content starts among Wanderers and Casual Browsers, leading to higher repeat engagement, improved retention, and lower churn.
- **Primary success metric the one number that defines success, from M3:** Start Rate = % of eligible Wanderer/Casual Browser homepage sessions resulting in playback starting.
- **Baseline rate today's rate of your primary metric, from your M3 data:** 29%
- **Guardrail metric & boundary what must not break, and how far it can move before you investigate:** Power User weekly sessions have to remain within 5% of the existing 4.8 sessions/week baseline.
- **Minimum Detectable Effect (MDE) the smallest improvement worth shipping, your floor:** +3 percentage points absolute (29% → 32%)
- **Sample size per arm use the calculator in the builder, baseline + MDE:** 3697
- **Traffic split & test duration 50/50 standard · cover ≥ 2 weekly cycles:** 50/50 over 2 weeks
- **Significance threshold p < 0.05 is standard, explain any deviation:** p < 0.05

## Define your control and variant
- **Control (A) the current experience, reference your M2 moment of misery and M3 funnel/workflow data:** Low-intent users use the existing StreamLine homepage and recommendation experience. Discovery often requires prolonged browsing, causing some users to return to familiar comfort shows or leave without starting anything new; current Start Playing rate is approximately 29%.
- **Variant (B) your single change, copy the relevant screens & functional requirements from your M4 PRD:** Add one human-curated Spotlight rail to the homepage.
- **Isolation check, what has NOT changed? list everything identical between arms (app version, recommendation engine, notifications, onboarding). If something changed inadvertently, your test is compromised.:** App version and underlying product experience remain identical between Control and Variant.
Existing recommendation algorithm remains unchanged; Spotlight does not replace or retrain it.
All existing homepage rows remain unchanged in content, order, and behavior, except space required for Spotlight.
Search experience remains identical.
Title-detail screen remains identical after a title is selected.
Play button and playback flow remain identical.
Playback quality, buffering, subtitles, and device support remain identical.
Content catalogue and availability remain identical; Variant does not receive exclusive titles.
Pricing, subscription plans, and promotions remain identical.
Notifications, emails, and external marketing remain identical.
Onboarding and login experience remain identical.
Account settings and preferences remain identical.
Viewing-history behavior remains identical; it is used only to avoid completed titles where available.
Recommendation personalization elsewhere in the app remains identical.
Power User experience outside Spotlight remains unchanged.
Analytics definitions for Start Playing and new-title starts remain identical between arms.

## Formalize your hypothesis & shipping criteria
- **Your hypothesis (filled in):** I believe that the Spotlight Curated Rail for low-intent Wanderers and Casual Browsers who want easy entertainment but rarely invest effort discovering something new will result in more successful transitions from homepage discovery to playback, as measured by a +3 percentage-point absolute increase in Start Rate, from 29% to 32%, within 14 days. We will protect Power User weekly sessions, ensuring they remain within 5% of the 4.8 sessions/week baseline throughout the test.
- **Your shipping criteria (filled in):** We will SHIP if Start Rate improves by ≥3 percentage points absolute at p < 0.05 and Power User weekly sessions do not fall below 4.56 sessions/week after 14 days, with the required sample of 3,697 observations per arm reached.

We will ITERATE if Start Rate moves positively but the lift is below +3 percentage points.

We will KILL if Start Rate shows no improvement or moves negatively.

The read date is fixed at the end of the 14-day test window, and no experiment results will be reviewed before that date.
- **Hardest parameter to define, and did it change your hypothesis? quick debrief:** Primary Metric was decently difficult to define back in M3, it did change my hypothesis a bit, also based on the Persona, since I had initially decided on a different one back in M2.
