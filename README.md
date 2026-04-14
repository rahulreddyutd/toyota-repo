# OAS Product Management Portfolio

Three tools I built to demonstrate how I think about the Operator Assist Systems PM role at TMHNA.

---

I spent time reading through the OAS PM job description carefully before building anything. The role asks for someone who can own competitive intelligence, build financial justification tools for the sales team, and drive a product roadmap from vision through launch. So that's exactly what I tried to show — not with slides or bullet points, but with working software.

Each tool is scoped to something real. The data comes from actual industry sources. The features in the roadmap are things a forklift OEM would genuinely be thinking about in 2025.

---

## The three projects

### 01 — Competitive Intelligence Dashboard

The job description mentions gathering and maintaining competitive intelligence as a core responsibility. I wanted to show I already know this market.

The dashboard tracks 12 competitors across three segments: forklift OEMs (Crown, Jungheinrich, Hyster-Yale, Linde, Mitsubishi, STILL), ADAS and sensor suppliers (Sick AG, Cognex), and software platforms (Seegrid, Zebra Technologies, Daifuku, Würth). Each competitor has a technology breakdown across LiDAR, computer vision, UWB, and radar, a feature depth score, estimated price range, market reach, and a threat assessment.

The part I think is most useful is the SWOT panel. Click any row and you get a quick read on what that company is actually good at, where they're weak, what opportunity that creates for TMHNA, and what risk they pose. The positioning map in the corner shows everyone plotted by feature sophistication versus price — useful for spotting white space.

I used public OEM product pages, dealer documentation, trade press coverage from DC Velocity and Modern Materials Handling, and MHI's 2024 annual report for the data.

### 02 — ROI & TCO Calculator

Sales reps need something they can put in front of a fleet manager that makes the investment decision obvious. That's what this is.

You enter your fleet size, shift pattern, incident history, insurance costs, operator wages, and downtime numbers. The calculator models what OAS actually does to those numbers — incident cost avoidance based on a configurable reduction rate, insurance premium savings, downtime reduction from fewer collision-related repairs, and throughput efficiency gains. It outputs annual net savings, 5-year NPV at an 8% discount rate, and payback period.

The framing I care about most is the "cost without OAS" number. Most conversations anchor on the price of the system. This tool reframes it: what are you already spending on incidents, insurance, and lost productivity? That number is almost always bigger than the OAS price tag, and it's usually the thing that moves a procurement conversation forward.

Incident cost data comes from Liberty Mutual's Workplace Safety Index. The 2.8% throughput efficiency figure is from MHI's Annual Industry Report. Insurance savings use a 55% multiplier against the incident reduction rate, which is based on NSC actuarial modeling. I tried to keep all the assumptions conservative so the numbers hold up when a CFO pushes back.

There's a print button that exports a clean PDF summary — the kind of thing a rep can leave behind after a site visit.

### 03 — Product Roadmap Planner

The roadmap covers 12 OAS features across FY2025, organized in a swimlane view by quarter. There's also a sortable feature list and a RICE score view that ranks everything by priority.

The features are things I genuinely think belong on an OAS roadmap right now: LiDAR v2 to close the false-positive gap with Sick AG's microScan3, UWB personnel detection to compete with Zebra MotionWorks on the brownfield retrofit side, computer vision pallet detection to go after Crown QuickPick Remote's market share, and an OAS API layer because 80% of enterprise RFPs I've seen in adjacent industries require WMS integration before procurement will even consider a system.

Click any feature card and you get the full detail — RICE breakdown with individual component scores, market rationale (what competitive signal or lost deal drove this), technical dependencies, and target customer segment. The RICE scoring is there because prioritization decisions are easier to defend when they're tied to something quantifiable. When Engineering asks why something got bumped to Q4, or Sales asks why their favorite feature isn't in Q2, you can point to a number instead of an opinion.

The filters let you view the roadmap by owner team or status, which is closer to how cross-functional planning conversations actually happen.

---

## Why I built it this way

I could have made slides. A competitive analysis deck, a financial model in Excel, a roadmap in a PowerPoint template. Those are fine, but they don't show how someone thinks about building tools for other people to use.

Everything here is built as something a real team could pick up and use. The ROI calculator is the kind of tool I'd want every sales rep to have open before a customer meeting. The competitive dashboard is the kind of thing I'd update quarterly and share before a business review. The roadmap has the detail a cross-functional team actually needs — not just feature names and dates, but the why behind each decision.

The industries are right. The terminology is right. The data sources are real. That's intentional.

---

Questions or feedback welcome — happy to walk through the thinking behind any of it.
