# Kaizen Case Studies: talk script (45 min)

Deck: https://claude.ai/artifact/63WW5ZguMhnfnAPjp9BBJ4 (31 slides)

**Shape:** 5 min about you → 20 min NITMRE FX → 18 min OMEN Design Studio → questions.
**Pace:** about 140 words a minute. Each section shows its target time; the running clock is in brackets.
**Honest timing:** the spoken words alone run about 4 minutes for Part 1, 12–14 for NITMRE and 12–13 for OMEN. Pauses, zoom clicks and the walkthroughs add the rest. Fill spare time with real questions mid-talk (invite them at the start), not extra words.
**Keys:** → or Space = next click · ← = back · Slides = jump to any slide · F = full screen.
`[→]` = press → to go on. 🔵 **`→ ZOOM 1: TABS`** = press → right there, mid-sentence, to zoom to that spot. **Bold** = the line to land. *Italics* = stage direction. ⚠ = a fact to settle before the call.

---

## Part 1 · About me (5:00)

### Slide 1 · Cover — 0:30 `[0:00–0:30]`

"Hi everyone, I'm Meghan Kulkarni. I'm a product designer, and I'm super excited to be talking with you about the Product Designer, Delivery role at Kaizen, and to get to know you all better.

I'll take a few minutes to explain who I am, and then walk you through two case studies: NITMRE FX, a flight planning tool I designed with the Air Force, and OMEN Design Studio. Please jump in at any point with questions.

Let's get right into it."

`[→]`

### Slide 2 · Swims and flies — 1:00 `[0:30–1:30]`

"Some personal background about me. **I love everything that swims.** I love the ocean, and I'm scuba certified. This is from my most recent trip to Bonaire, where I actually got to see a barracuda in the wild, which was super cool.

*(point right)* **And I love everything that flies.** I'm a student pilot, training for my private pilot license. That's me flying a Tecnam Astore. And it's not a coincidence that my most recent product design work has been designing for aerospace."

`[→]`

### Slide 3 · Kaizer — 0:30 `[1:30–2:00]`

"And at home, I have a cat. **His name is Kaizer.**

*(beat)* Which is one letter off from Kaizen…"

*(Let them laugh. Don't explain it.)*

`[→]`

### Slide 4 · Background — 2:15 `[2:00–4:15]`

"Getting into my professional background.

I'm a product designer at Airspace Intelligence, designing across three domains: defense, commercial aviation, and, more recently, energy.

On the defense side, I work really closely with the Air Force, on both sortie planning and mission operations. The project I will be walking you through today is sortie planning.

On the commercial side, it's mostly air traffic control applications. I've also worked on Flight Deck, which helps pilots reroute and reconfigure their routes based on dispatcher communication. It runs on an iPad they have with them in the cockpit. **And most of the major airlines use Flight Deck now.**

Before Airspace Intelligence, I was the founding product designer at Accrete AI, a B2B SaaS company with a government subsidiary. On the government side, I worked with the Department of Defense on threat detection software and defense intelligence.

*(Why defense, about 30 seconds)*

I actually ended up in defense pretty randomly. **But I kept choosing it because of the people I get to design for.** The users are accountable. They have to make decisions within seconds in mission-critical environments. That changes the scope of things, because **design isn't a nice-to-have, it's the trust-building mechanism.** It's about surfacing the right information, so they can make the call and trust the product enough to act on it. That's what keeps me in defense.

Before defense, I was briefly at a Kubernetes company, and I started my career in food and beverage at Keurig Dr Pepper, on their website and mobile app."

`[→]`

### Slide 5 · NITMRE FX Flight Planning — 1:00 `[4:15–5:15]`

"The first case study is a project where trust was the whole design problem: NITMRE FX Flight Planning.

For context, the client here is U.S. Air Force Air Mobility Command, the part of the Air Force that moves people, cargo and fuel. **NITMRE FX is a flight planning tool for their flight managers.** Flight managers plan sorties, which are individual mission flights, like a tanker on a refueling run, and they sign off on every number in the plan. FX replaces the legacy tools they used to do that, so they can verify a plan faster and more accurately.

**We designed and built this product from zero to one.** I was the product designer, working with a team of engineers and a deployment lead, who's also an expert in this domain."

`[→]`

---

## Part 2 · NITMRE FX (20:00)

### Slide 6 · Problem and goal — 2:30 `[5:00–7:30]`

"So, to set the scene and really frame the problem: **whenever you plan a sortie, like a refueling mission for a tanker, it takes two to three hours, and you're toggling across six to seven legacy tools that have no connection to each other.**

Some of these tools are super dense. They're literally blocks of information you have to comb through to find very specific statuses. There are manual calculations, like passenger and cargo weight, that live in dense Excel sheets. You also have important remarks and critical operational information buried in free text. So it's a pretty complex workflow, and it takes a lot of time.

But that's only one sortie. A mission has several sorties, so some days there are a lot of them to plan. That's just not effective, especially in mission-critical situations where time is key.

The other problem: there's only a very small group of flight managers who actually know how to plan sorties. Take one flight manager, and we'll call him Earl. *(beat)* Earl has worked with the Air Force for decades, and he's ready to retire. **But he's one of the only people who knows how to plan sorties.** A lot of the flow and information lives in his head, so there's no easy way to onboard new flight managers. So Earl just hasn't been able to retire…"

*(Let it land.)*

`[→]` *(Goal row appears)*

"So that leads us to our goal: **replace all of those legacy tools and all that dense information with one intuitive workflow.** It should be faster. It should automate some of those calculations. It should be easy to onboard onto. And most importantly, **it has to be compliant**: every route has to meet its clearances.

*(beat)* And it'll help Earl retire."

`[→]`

### Slide 7 · Two days at their desks — 1:00 `[7:30–8:30]`

"So in July, we had the opportunity to spend two days on site with flight managers at an Air Force base. **We watched them plan sorties in real time.** We sat next to them while they worked, asked them to talk us through their workflow as they were doing it, and I noted every point where they stopped to check something, or anywhere there seemed to be friction.

*(point at the diagram, left to right)* So this is the workflow. Several legacy tools. Dense Excel sheets for weight. Remarks in free text. And, most shockingly, **SkyVector to double-check it.** SkyVector is a free website that pilots use for flight charts. We're going to talk a little bit more about that. But once you have the configured route, it gets pasted into GDSS, which is the Air Force's system of record."

`[→]`

### Slide 8 · Insight — 1:30 `[8:30–10:00]`

"That SkyVector moment really stuck with me. *(point at the screenshot)* A flight manager finishes a route in their tools. Then, before trusting that route they just built, they open SkyVector and trace the same airway by eye. Their tools were so outdated that expert Air Force planners needed a free chart site just to feel confident in a route.

That's when it clicked:

**flight managers aren't looking for an answer. They're checking one.**

*(pause)*

Which means, even if we automated it and recommended routes for their sorties, a route they can't check doesn't save time. It's just one more thing to verify.

So we went in asking, *what can we automate?* And I came out asking, **what do they need to verify, and how fast can we make that?** That became my North Star."

`[→]`

### Slide 9 · Five places checking slowed them down — 0:45 `[10:00–10:45]`

"All right. So if the job is checking, **where did checking take the most time?** I identified five places while observing their workflows.

Let's go through them."

`[→]`

### Slide 10 · Challenge 1: a guided planning mode — 1:30 `[10:45–12:15]`

"The first challenge: **scattered tools with no clear, documented order.** While they're building a route, nothing tells them which tool to use next, or what step comes after.

But as we watched, every flight manager worked through a sortie in a similar pattern. **Pre-plan** the clearances, aircraft and crew. Calculate the **weight**. Build the **route**. Check the **airfields**. Then **export** to GDSS.

That pattern wasn't written down anywhere. It lived in the flight managers' heads, and in Earl's.

So **I made planning its own guided mode, built around that pattern.** 🔵 **`→ ZOOM 1: TABS`** Their steps become the tabs at the top. You have your pre-plan first, where you look at remarks. Then you move to routing, and each section gets confirmed before you move on. 🔵 **`→ ZOOM 2: ACTION BAR`** And it ends in an action at the bottom: evaluate, compare, export, with a route ready for GDSS.

So **it reads like a checklist they confirm, step by step, not a blank canvas.** And for a new flight manager, the pattern Earl kept in his head is now right there on screen."

`[→]`

### Slide 11 · Challenge 2: summary and clear statuses — 2:00 `[12:15–14:15]`

"The next slowdown was finding *what* to check. **Statuses were buried in dense documents.**

Most of planning is confirming that each condition is fine. I didn't want them reading paragraphs to find the one problem. So the plan is **summarized up front** 🔵 **`→ ZOOM 1: SUMMARY`**: fuel burn, flight time and landing. **And every check has a clear status, cleared or not cleared.** 🔵 **`→ ZOOM 2: CHECKS`** Each compliance check, like NATS and DIPS, carries its own state. Here, DIPS, your diplomatic clearance, is not cleared, so the flight manager can investigate it.

🔵 **`→ ZOOM 3: REMARKS`** And remarks that matter surface up front, ranked by how critical they are. **Magenta is the most critical.** No more hiding in free text.

**They scan the states, and spend their attention only where something needs it.**"

`[→]`

### Slide 12 · Challenge 3: show the source — 1:45 `[14:15–16:00]`

"Seeing a status wasn't enough, though. To be confident in a route, they had to check every calculated value for accuracy, and **track down which sources these values came from.**

*(slow down; this is the strongest point)*

So **every value traces back to its source.** A confident number isn't enough. Trust comes from being able to check the math.

🔵 **`→ ZOOM 1: DATA SOURCES`** You have your breakdown for your requirement values here, and one click into the details shows the math and the sources. So instead of opening a spreadsheet to rebuild a number, the flight manager can check it right where they're signing. 🔵 **`→ ZOOM 2: GATES`** Same interaction for your payload values: one click shows that they come from GATES, and when they were last modified.

**Honestly, without mapping to the source of truth, nothing else on this screen would actually matter.**"

`[→]`

### Slide 13 · Challenge 4: a weight builder — 1:45 `[16:00–17:45]`

"Let's talk about automation, which is our fourth challenge. The catch: **anything the system calculates is one more thing to check.**

Weight was the obvious thing to automate. We could have calculated it for them. But the flight managers are still going to recalculate and double-check the calculations, so it isn't improving anything.

So I made **a weight builder, not a weight calculator.** I automated the gathering, not the judgment. Values are auto-filled from their sources, and there are configuration presets to start from. 🔵 **`→ ZOOM: PRESETS`** They pick a preset, then configure it, and make manual changes. Faster than Excel, and it's still theirs. They have full agency. The flight manager assembles it and signs it.

So essentially, **checking becomes a glance, not a recalculation.**"

`[→]`

### Slide 14 · Challenge 5: trusted routes kept intact — 1:15 `[17:45–19:00]`

"The last one is about trust. **To check a new route, flight managers need a route they already trust to check it against**, like one that's been flown before.

So **external, recommended and historically flown routes can't be edited directly.** 🔵 **`→ ZOOM 1: COPY`** They duplicate one and edit the copy, so the original stays intact. 🔵 **`→ ZOOM 2: SIDE BY SIDE`** Then they compare them side by side: burn, time and every check.

**The route they trust is always there to check against.**"

`[→]`

### Slide 15 · Outcome — 1:00 `[19:00–20:00]`

"Here's what all of this added up to.

*(point left)* So before: two to three hours, too many tools, and several workflows.

`[→]`

*(point right)* After: **one tool, fifteen to twenty minutes, and one workflow** in NITMRE FX. Checked, signed, and into GDSS.

I typically build things in code, but for engineering handoff, I built a Figma prototype. Air Force workflows, routes and clearance details can't go into AI coding tools, so a prototype with sample data avoided that entirely. For handoff, I built out the components engineering needed, like the panels, with all of their states: default, hover and selected. So engineering could build straight from the Figma files.

The MVP shipped in August, we briefed the full flow on site in September, *(beat)* and Earl could finally retire."

`[→]`

### Slide 16 · What I'd do differently — 1:30 `[20:00–21:30]`

"Two things I'd do differently.

**First, I'd watch newer flight managers, not just the experts.** The people we watched were experienced, and Earl knew everything. But someone newer can show you exactly where the workflow is hard to learn. And that is the problem when the expert retires.

**Second, I'd design for when things go wrong, earlier.** Sometimes you could have a situation where two sources disagree on passenger weight. The tool should be able to flag the disconnect between those two sources. And if a check like diplomatic clearance can't load, it should say *can't verify* instead of quietly showing cleared."

`[→]`

### Slide 17 · Walkthrough — 1:00 `[21:30–22:30]`

"Here's the whole flow, start to finish."

*(It plays on its own, about 40 seconds a loop, 5 seconds a step. Let it loop and talk over it; click the frame to pause on a step.)*

1. "They open planning right from the sortie."
2. "Pre-plan first, in their order. Remarks sit with each leg instead of buried in free text."
3. "Then they add a route…"
4. "…usually starting from a historical route they already trust."
5. "Weight fills in from the source data. They pick presets and adjust."
6. "Evaluate. Every check comes back cleared or not cleared, and they can see why."
7. "They compare it against the historical route…"
8. "…and export it into GDSS. That's the whole sortie, in one place."

`[→]`

*(About 2:30 of buffer for questions before OMEN at 25:00. Then: "That's NITMRE FX. The second project is a very different kind of design problem.")*

---

## Part 3 · OMEN Design Studio (18:00)

### Slide 18 · OMEN Design Studio — 1:00 `[25:00–26:00]`

*(Coming off the NITMRE walkthrough.)*

"So the second project I want to show you is OMEN Design Studio, which I built at Airspace Intelligence as well.

The client here is the U.S. Air Force. **I was the only product designer**, and I worked with a team of engineers and a deployment lead. ⚠

So, high-level context: **OMEN Design Studio is where Air Force squadrons can customize and plan their own applications to build missions.** This can include combat missions, surveillance missions, any type of mission. ⚠"

`[→]`

### Slide 19 · Original goal, why I switched, new focus — 1:45 `[26:00–27:45]`

"I'd only been at ASI about two weeks when a pitch came up for DIU, the Defense Innovation Unit. ⚠

You have **two separate user groups.** The first is a squadron officer: doesn't write code, but knows exactly what the mission needs. The second is an engineer, wiring up new data feeds.

**So the goal was to provide an experience for both engineers and officers to plan missions.**

And the requirements were all about the technical platform: running the apps, connecting the data, meeting the security rules."

`[→]` *(Why I switched appears)*

"But here's what I kept seeing. In the Air Force, **every squadron wants its app slightly different.** Some of it is the type of mission they're flying, some of it is how they like to work, and there are good reasons for all of it.

But **every single difference meant new code and a new build.** And in a classified environment, a new build can take weeks to deploy. ⚠ So something as small as *can we move this panel over here?* was slow and expensive.

**Nobody had asked for a way to change the apps without an engineer.** But it was really clear to me that the people using them needed one."

`[→]` *(New focus appears)*

"So that became my focus: **a Design Studio.** Build once, and let mission owners configure their own apps, with no code.

*(beat)* Nobody had asked for it, and we had two weeks."

`[→]`

### Slide 20 · Two weeks, five questions — 0:45 `[27:30–28:15]`

"In two weeks, I obviously couldn't design everything. So I spent the time on a few questions, and **I'll walk you through how I thought about each one**, because that's where those two weeks really went."

*(Point down the list; don't read all five.)*

`[→]`

### Slide 21 · Question 1: one product, two skill levels — 1:30 `[28:15–29:45]`

"The first question was: **who exactly is this for?** Remember those two users: the squadron officer who just wants to move a panel or add a layer, and the engineer wiring up a brand-new data feed.

At first glance, the obvious option is two products: a simple one for officers, and a developer tool for engineers. **But what I kept coming back to was that they're working on the same app.** Two tools means two sources of truth, and a lot of back and forth just to keep each other up to date.

**So I pushed for one product with two skill levels.** Every other decision follows from this one."

`[→]`

### Slide 22 · Question 2: never start from a blank screen — 1:30 `[29:45–31:15]`

"For the officer, the next question was: **where does someone who doesn't code get stuck?**

Our Deployment Lead was a lieutenant, so they were essentially our stand-in user. ⚠ And the answer was the very first screen. **A blank canvas is flexible, but it's exactly where people freeze**, or build something that doesn't work.

So the decision: **you never start from a blank screen.** 🔵 **`→ ZOOM 1: MISSION TEMPLATES`** The App Builder opens on mission templates. 🔵 **`→ ZOOM 2: MOVING MAP`** You pick one, like this moving map, ⚠ and **you're looking at a working app on the very first click.** Every change after that is a small edit to something that already works."

`[→]`

### Slide 23 · Question 3: one pattern for every component — 2:00 `[31:15–33:15]`

"The next question was: **what will people remember between uses?**

These aren't people who live in this tool. **There are no power users.** They open it when they're building a mission, or when a mission changes.

🔵 **`→ ZOOM 1: CLICK THE COMPONENT`** So say I want to change the toolbar. I click it, 🔵 **`→ ZOOM 2: THE PANEL`** and the panel on the right shows me that component: what's on it, what's available to add, and I drag to reorder. No code.

And the mission card works **the exact same way.** Click the component, and the panel shows you that component and what you can change.

I could have given each component its own editor, more tuned to that component. **But I weighed that against someone coming back after a month or two and having to relearn it.** With one pattern, once you've learned one component, you've learned them all."

`[→]`

### Slide 24 · Data without code — 1:30 `[33:15–34:45]`

"Next is data. In these apps, **data is the hardest part, and it's usually where an engineer has to step in.** Every layer on the map, like weather, tankers or airports, is a data feed someone has to wire up.

So the question I asked was: **how would an officer look for data?** Not by feed name or endpoint. They think in terms of what they want to see on the map.

🔵 **`→ ZOOM 1: CATEGORIES`** So the catalog is organized the way they think. Map layers, like weather and winds. Moving assets, like tankers and fighters. Static ones, like airports and waypoints. And services, like fuel burn.

🔵 **`→ ZOOM 2: ONE ROW`** Each category has its own setup, because **setting up a weather overlay is a very different job from tracking an aircraft.**

*(point at NEW, top right)* And if what you need isn't in the catalog, you build your own layer."

`[→]`

### Slide 25 · Question 4: no code and code are one definition — 1:30 `[34:45–36:15]`

"If the catalog doesn't have what you need, you build your own layer. And this is where the next question comes in: **how do the officer and the engineer actually work on the same thing?**

Normally, adding something to the map means an engineer writes code. 🔵 **`→ ZOOM 1: STEP BY STEP`** **Here, you connect a data source and tell the map what each part means**, step by step. 🔵 **`→ ZOOM 2: HOW IT LOOKS`** Then you pick how it looks: name, color and icon, and you see it on the map as you go.

🔵 **`→ ZOOM 3: CODE TAB`** And for the engineer, **the exact same layer is one tab away, as code.**"

`[→]`

### Slide 26 · Two views of the same layer — 1:15 `[36:15–37:30]`

🔵 **`→ ZOOM 1: CODE`** "Here's that same layer, as code. 🔵 **`→ ZOOM 2: MAP PREVIEW`** The map previews the result, 🔵 **`→ ZOOM 3: ERRORS`** and any errors show up right underneath.

The usual answer here is a no-code builder for some people and a separate code path for others. **But in a mission-critical environment, a lot can go wrong with that.** Someone edits the code, and suddenly the visual version is wrong.

**So I made them two views of one definition.** The officer and the engineer are editing the same thing, at the level each of them is comfortable with."

`[→]`

### Slide 27 · Question 5: show what's in a version before it ships — 1:45 `[37:30–39:15]`

"Everything you build here is headed for a mission, for an aircraft. So the last question was: **what do you need to know before you hit publish?** You can't put blind trust in what you've built.

Security could have stayed behind the scenes, checked by someone else after it's published. **But I'd just handed people the power to change a mission app themselves.** So I thought they should also see exactly what they're shipping.

🔵 **`→ ZOOM 1: WHICH VERSION`** So before you publish, you see exactly what's in the version. 🔵 **`→ ZOOM 2: BY SEVERITY`** The findings by severity, 🔵 **`→ ZOOM 3: EACH VULNERABILITY`** **all the way down to each individual vulnerability**, with a plain explanation of what it means and what you can do about it.

**Publishing should be a confident decision, not a leap of faith.**"

`[→]`

### Slide 28 · Outcome — 1:15 `[39:15–40:30]`

"Here's what that added up to.

*(point at Before)* Before: a squadron request meant new code and a new build, and **weeks** to deploy."

`[→]`

"*(point at After)* After: **the mission owner makes the change in the Design Studio, and it's saved to the app.** No code.

I designed it in two weeks for the DIU pitch. ⚠ At the first outside demo, three Air Force users went from **'you can skip the design studio'** to **'when can we use that?'**, the same day. *(beat)* And **OMEN went on to win part of a $21 million DIU award**, shared with two partner companies. ⚠"

`[→]`

### Slide 29 · What I'd do differently — 1:15 `[40:30–41:45]`

"Two things I'd do differently.

**First, I'd test with squadron officers, not just a stand-in.** Our Deployment Lead was a great proxy, but the first real reaction from the people who'd use it came at the demo. I'd want that much earlier.

**Second, I'd show the data before it's connected.** Data previews are still on the roadmap. I'd bring them into the first version, so people can trust what they've connected before it's on the map."

`[→]`

### Slide 30 · Walkthrough — 1:15 `[41:45–43:00]`

"And here's the whole flow, start to finish."

*(It plays on its own, 5 seconds a step, about 45 seconds a loop. Talk over it; click the frame to pause on a step.)*

1. "You start from a mission template…"
2. "…and you're looking at a working app on the first click."
3. "Click a component, and you configure it on the right."
4. "Same pattern for every component."
5. "Pick data from the catalog, or build something new."
6. "Build a layer step by step, no code…"
7. "…and the engineer sees the same layer, as code."
8. "When a security update is ready…"
9. "…you see every finding before you publish."

`[→]`

### Slide 31 · Thank you — 0:15 `[43:00–43:15]`

"Thank you. I'd love to hear your questions."

*(Stop. Don't add a summary.)*

---

## If they push on OMEN

- **"What exactly was yours?"** "I designed the studio for the pitch, as the only product designer, working with the engineers and our Deployment Lead."
- **"Did you win the award?"** "OMEN won part of a $21 million DIU award, shared with two partner companies. I designed the studio that was part of the pitch."
- **"Was it user-tested?"** "Not formally. Our Deployment Lead was a lieutenant, so they were our stand-in user, and the reaction from Air Force users at the first demo was the strongest signal." *(That's why it's first on your reflection slide.)*
- **"Which decision was hardest?"** ✎ Your pick. Question 3 is a good one: one pattern costs a little on each component, and you have to hold the line on it.
- **"Is it live?"** "Not on aircraft yet. Publishing to the aircraft, data previews and a chat assistant are on the roadmap."
- **"How does this relate to Kaizen?"** ✎ Your call. The parallel is real: OMEN lets people who don't code shape the software they depend on, without waiting on an engineering cycle.

---

## Part 4 · Questions

Click **Slides** to jump back to any screen. Slide 9 (Five places) and slide 20 (Five questions) are clickable: each row jumps to its slide.

**Likely questions and short answers**

- **"How was 15–20 minutes measured?"**
  Say only what's true: *"We timed flight managers on site…"*, or *"That's what flight managers reported…"*, or *"It's the team's estimate from walking the full flow."* Don't round up.
- **"What was you versus the team?"**
  "I" for the design decisions, the UI guidelines engineering built from, and running the design sessions. "We" for the site visits and shipping.
- **"How did you identify the five challenges?"**
  "While we watched them plan real sorties, I noted every point where they stopped to check something: switching tools, digging through a document, re-doing a calculation, opening another site. Afterwards I grouped those moments, and they clustered into five places." *(Adjust to what you actually did: notes, timestamps, an affinity map.)*
- **"How did you automate without adding checking?"**
  "I automated the gathering, not the judgment. Auto-filled values with their sources, and presets. The flight manager assembles and signs it."
- **"Why a Figma prototype, if you usually build in code?"**
  "Mainly the data. Air Force workflows, routes and clearance details can't go into AI coding tools or outside services, so a Figma prototype with sample data avoided that entirely. And engineering built straight from the Figma files, so it was also the handoff. If I'd coded it, the team would have had a second source of truth to translate back."
- **"Why defense?"**
  The 30-second answer from slide 4.
- **"Can we see more?"**
  "Happy to walk through any screen in more depth." Keep detail at the level on the slides because of confidentiality.
- **"Is using SkyVector a security issue?"**
  Only if you know: "They used it to look, not to plan."

---

## Before the interview

1. **Time it out loud once.** If you run long, trim slide 11's zooms first, then OMEN's slide 26.
2. **Confirm the facts you'll be asked about:** how 15–20 minutes was measured; what DIPS, NATS and GDSS meant on your team; whether Earl is a real name (if so, consider "let's call him Earl").
3. **Practice the clicks.** Several slides zoom on →, so → doesn't always move to the next slide. Press it until the zooms finish.
4. **Share the deck** from the artifact's Share menu if anyone needs the link.
5. **Clear the walkthrough frames.** Slides 17 and 30 use screens from the Figma prototype in Airspace Intelligence's Figma. Check that showing them is within your confidentiality agreement.
6. **Some lines are drafted, not quoted.** The walkthrough lines on slides 17 and 30 are my wording. Change anything that isn't exactly how it happened.

---

## ⚠ Settle before the call (OMEN)

1. **DIU is the Defense Innovation Unit**, not "Defense Intelligence Unit." Interviewers in govtech will notice.
2. **Don't claim the whole award.** OMEN won **part of** a $21M award, shared with two partner companies.
3. **"Two weeks."** You designed it in two weeks; engineering had it working in about two and a half. If asked, say two weeks to design.
4. **"Weeks to deploy."** The case study says weeks. Only say "months" if you know it's true.
5. **The Deployment Lead as a lieutenant.** Check that their rank is fine to say.
6. **"Moving map."** Check the template name is fine to say under your PIIA.
7. **Walkthrough lines are my wording.** Change anything that isn't exactly how it happened.
