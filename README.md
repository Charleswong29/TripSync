# 🌍 TripSync by VEGE LLAO²

> **Find people. Plan together. Travel better.**

**Team Member :** Celine Hew Boon Ling, Kok Jia Hui, Siew Hoi Wei, Wong Chee Yong  
**Problem Statement :** Travel Planner  
**Video Presentation :** []  
**Presentation Slides :** []

---

# 1. Project Overview

## ✈️ The Problem

Planning a trip becomes more difficult when multiple people are involved.

Travellers may have different budgets, interests, travel pace, food preferences, transportation preferences and must-visit places. This often makes group decision-making difficult, and one person may end up doing most of the planning.

Solo travellers may face another problem: they want to travel but do not have a suitable travel companion because their friends may be unavailable, have different budgets or prefer different travel styles.

Travel information is also scattered across different platforms. Travellers may need separate applications or websites for attractions, accommodation, transportation, restaurants and itinerary planning.

Finally, most travel plans are static. Unexpected situations such as bad weather, delays, overspending, tiredness, attraction closures or changes in group members can make the original itinerary unsuitable.

### Existing Solutions

One existing solution is **Wanderlog**, which provides itinerary planning, real-time collaboration, budgeting, route optimisation and AI-assisted travel planning.

However, TripSync focuses on a different part of the group travel problem: helping users **find compatible travel companions, reach agreement fairly, and adapt the group's plan when circumstances change**.

Instead of focusing only on:

> "Where should we go?"

TripSync also asks:

> "Who should we travel with?"  
> "How can everyone agree?"  
> "What happens when the original plan no longer works?"

---

## 💡 Our Solution

**TripSync** is an AI-powered group travel planner and travel teaming platform.

It connects the entire group travel journey through four stages:

**Find → Agree → Plan → Adapt**

Users can create a public trip to find compatible travel companions or create a private trip for family, couples and friends. Group members provide their travel preferences and vote on activities before TripSync generates an itinerary that considers budget, time, transportation and group preferences.

When something unexpected happens during the trip, **Plan Rescue** adjusts the affected part of the itinerary instead of requiring users to start planning again.

### Core Features

- 👥 Public & Private Trips
- 🔎 Travel Teaming
- 🧩 Travel Compatibility Matching
- 🎭 Travel Personality & Preference Profile
- 🗳️ Swipe & Vote
- ⚖️ Group Fairness Meter
- 🤖 AI Smart Itinerary
- 💰 Budget Dashboard
- 🚨 Plan Rescue
- ❤️ Favourite Travel Buddies

---

# 2. Ideation & Process

## 2.1 Ideas We Considered

During brainstorming, we explored different ways of solving problems that occur before, during and after group trip planning.

| **Idea** | **Why it was dropped / kept** |
|---|---|
| **Plan Rescue (Chosen)** | **Kept.** Most travel planners focus on creating an itinerary. We wanted TripSync to continue helping after the trip begins. Plan Rescue adjusts affected activities when situations such as weather, delays, budget problems or closures occur. |
| **Travel Teaming (Chosen)** | **Kept.** We realised that some users, especially solo travellers and students, may want to travel but do not have a suitable travel companion. Public Trips allow users to discover potentially compatible travel groups. |
| **Group Preference Matching (Chosen)** | **Kept.** Different group members may have different budgets, interests and travel styles. Combining preferences into a Group Profile helps TripSync understand the group. |
| **Swipe & Vote (Chosen)** | **Kept.** Instead of allowing one person to control the itinerary, members can vote on suggested activities using Must Go, Like, Neutral and Skip. |
| **Group Fairness Meter (Chosen)** | **Kept.** Majority voting can repeatedly ignore the same member. The Fairness Meter helps identify members whose preferences are underrepresented. |
| **Travel Personality (Chosen)** | **Kept.** A simple preference profile helps calculate compatibility between travellers and provides information for itinerary generation. |
| **Smart Budget Guard (Chosen / Simplified)** | **Kept but simplified.** Budget is important, especially for student travellers. For the prototype, we focus on planned, spent and remaining budget rather than complex financial optimisation. |
| **People Tags & Favourite Travel Buddies (Optional)** | **Kept as a secondary feature.** Users can identify people as Family, Friend, Partner, Classmate or Travel Buddy and reconnect with compatible travellers in future trips. |
| **Real-time Weather Detection** | **Simplified for MVP.** Automatic detection requires additional API integration. The prototype can demonstrate Plan Rescue by allowing users to select "Bad Weather", with live weather integration planned later. |
| **Full Route Optimisation** | **Future development.** Optimising traffic, opening hours, distance, preferences and time simultaneously would make the prototype unnecessarily complex. |
| **Hotel / Flight / Bus Booking** | **Future development.** Booking requires external providers, availability data and additional API integration. It is outside the current core experience. |
| **Payment System** | **Future development.** Payments introduce additional security, transaction and integration requirements. |
| **Travel Marketplace** | **Future development.** It has business potential but would distract from validating TripSync's main group planning experience during the competition. |
| **AR Navigation** | **Dropped.** Interesting but does not directly solve TripSync's main problem of group coordination and itinerary adaptation. |
| **Full Social Media / Chat System** | **Dropped for MVP.** TripSync is not intended to become a general social network. Basic travel teaming and invitations are enough to test the core concept. |

---

## 2.2 Ideation Boards

### 🧠 Initial Mind Map

<img width="1336" height="824" alt="MAP 1" src="https://github.com/user-attachments/assets/e8a3474e-cbf8-4e62-b125-34fe90bbc4af" />

[Initial TripSync Mindmap]

*This mind map shows our early exploration of the Travel Planner problem, including itinerary generation, budgeting, group preferences, voting and unexpected travel situations.*

### 🌳 Problem Tree

<img width="1536" height="1024" alt="MAP 2" src="https://github.com/user-attachments/assets/b2b66b83-59e1-4ac5-a5c3-74f5f0effe1d" />

[TripSync Problem Tree]

*The problem tree explores the causes of stressful group travel planning, including conflicting preferences, scattered travel information, planning burden and unexpected changes.*

### 🔄 Idea Evolution

<img width="1536" height="1024" alt="MAP 3" src="https://github.com/user-attachments/assets/0a36d32d-389d-4ee7-a205-7300a7f0820a" />

[TripSync Idea Evolution]

*TripSync evolved from a basic AI itinerary generator into a group-focused platform that supports travel teaming, group agreement and adaptive planning.*

### 👤 User Flow

<img width="1536" height="1024" alt="MAP 4" src="https://github.com/user-attachments/assets/a834e5dc-d713-4929-ab18-971dfcc30e42" />

[TripSync User Flow]

*The user flow demonstrates the complete journey from finding or creating a trip to generating an itinerary and using Plan Rescue when circumstances change.*

---

### Our Idea Evolution

#### Version 1 — AI Travel Planner

Our initial idea focused mainly on generating an itinerary based on destination, budget and user preferences.

**Problem we identified:**  
AI itinerary generation alone was not sufficiently differentiated from existing travel planning solutions.

#### Version 2 — Group Travel Planner

We expanded the idea with:

- Group preferences
- Swipe & Vote
- Group Match Score
- Budget management

**Why we changed it:**  
We found that group decision-making was an important problem that a simple itinerary generator did not fully solve.

#### Version 3 — Adaptive Group Travel Planner

We introduced:

- Group Fairness Meter
- Plan Rescue
- Budget-aware alternatives

**Why we changed it:**  
We wanted TripSync to remain useful after an itinerary had already been generated.

#### Version 4 — Travel Teaming + Group Planning

We expanded TripSync further with:

- Public Trips
- Private Trips
- Travel Compatibility
- Favourite Travel Buddies

**Why we changed it:**  
We realised that some users face a problem even before planning begins: **they may not have suitable people to travel with.**

This led to our current positioning:

> **Find people. Plan together. Travel better.**

---

## 2.3 Mentor Consultation

| **Date** | **Mentor** | **Feedback Received** | **What Was Changed** |
|---|---|---|---|
| [TODO] | [TODO] | [Write the mentor's actual feedback] | [Explain what your team changed] |
| [TODO] | [TODO] | [Write the mentor's actual feedback] | [Explain what your team changed] |
| [TODO] | [TODO] | [Write the mentor's actual feedback] | [Explain what your team changed] |

> **Note:** This section will only contain actual mentor feedback received by the team.

---

# 3. Design & Prototype

**UI Prototype:** [TODO: Public Figma / Canva / Prototype Link]

Our prototype follows the complete TripSync user journey:

### 1. Welcome / Explore Trips
Users can discover a public trip or create their own trip.

<img width="540" height="870" alt="Screenshot 2026-09-11 003021" src="https://github.com/user-attachments/assets/0e609824-f1d2-4d2d-9b22-ae692f67d3b1" />

![Welcome Screen](assets/welcome.png)

### 2. Create Trip
Users select Public or Private Trip and enter destination, dates, budget and member limit.

<img width="555" height="881" alt="Screenshot 2026-09-11 003208" src="https://github.com/user-attachments/assets/26adaf56-232a-4eca-bf8e-1199ece041cd" />

![Create Trip](assets/create-trip.png)

### 3. Travel Personality
Users provide interests, food preferences, travel pace, transportation preferences, must-visit places and things they want to avoid.

![Travel Personality](assets/travel-personality.png)

### 4. Group Lobby
Shows members, compatibility scores and options to invite or apply to join.

<img width="552" height="876" alt="Screenshot 2026-09-11 003422" src="https://github.com/user-attachments/assets/27112b04-adcb-4457-a238-788da9a5740b" />

![Group Lobby](assets/group-lobby.png)

### 5. Swipe & Vote
Members vote on attractions using:

❤️ Must Go  
👍 Like  
😐 Neutral  
👎 Skip

<img width="535" height="868" alt="Screenshot 2026-09-11 003450" src="https://github.com/user-attachments/assets/257cf6e4-61d5-4df2-8379-5bc556b5be0f" />

![Swipe and Vote](assets/swipe-vote.png)

### 6. Group Match & Fairness

TripSync combines group preferences while also showing whether each member is fairly represented.

<img width="550" height="882" alt="Screenshot 2026-09-11 003522" src="https://github.com/user-attachments/assets/c01d488b-1024-4fe3-b589-d81531bd0ffa" />

![Group Match](assets/group-match.png)

### 7. Smart Itinerary

The generated itinerary displays:

- Time
- Activity
- Estimated cost
- Transportation
- Group Match

![Smart Itinerary](assets/smart-itinerary.png)

### 8. Budget Dashboard

Users can view:

- Planned budget
- Estimated spending
- Amount spent
- Remaining budget

![Budget Dashboard](assets/budget-dashboard.png)

### 9. Rescue My Day

Users select what went wrong:

- 🌧️ Bad Weather
- ⏰ Running Late
- 💸 Over Budget
- 😴 Too Tired
- 🚫 Place Closed
- 👥 Group Changed

TripSync then adjusts the affected section of the itinerary.

![Plan Rescue](assets/plan-rescue.png)

---

# 4. What Makes It Different

TripSync is not designed as only another AI itinerary generator.

Its main differentiation is connecting **travel teaming, group decision-making and adaptive itinerary planning** in one experience.

## 🔎 1. Travel Teaming

Users can create a **Public Trip** and allow compatible travellers to apply to join.

Compatibility can consider:

- Destination and date
- Budget range
- Interests
- Travel personality
- Travel pace
- Wake-up time
- Transportation preference
- Must-visit and avoid preferences

Private Trips remain available for existing groups such as families, couples and friends.

---

## ⚖️ 2. Group Fairness Meter

Normal majority voting may repeatedly favour the same people.

TripSync therefore evaluates how well the final itinerary represents each group member.

Example:

| Traveller | Itinerary Satisfaction |
|---|---:|
| Member A | 92% |
| Member B | 81% |
| Member C | 67% |
| Member D | 45% |

If one member is significantly underrepresented, TripSync can recommend an activity that better matches that person's interests.

---

## 🚨 3. Plan Rescue

Plan Rescue is TripSync's signature adaptive feature.

Instead of rebuilding an entire trip when something goes wrong, TripSync focuses on the affected section.

Example:

**Original**

`10:00 AM → Outdoor Attraction`

**Situation**

`🌧️ Bad Weather`

**TripSync**

`Outdoor Attraction → Nearby Indoor Alternative`

The system considers:

- Group preferences
- Available time
- Budget
- Activity type
- Location

before suggesting the replacement.

---

## 🎮 4. Game-Like Group Formation

TripSync takes inspiration from the idea of forming a team in multiplayer games.

Instead of:

> Find players → Create team → Play

TripSync applies:

> Find travellers → Form group → Agree → Travel

This provides a different approach to solo and group travel planning.

---

## Comparison with Existing Solutions

| Capability | Wanderlog | TripIt | TripSync |
|---|:---:|:---:|:---:|
| Itinerary management | ✅ | ✅ | ✅ |
| Group collaboration | ✅ | Sharing | ✅ |
| Budget support | ✅ | — | ✅ |
| AI-assisted planning | ✅ | Limited / different focus | ✅ |
| Find new travel companions | — | — | ✅ |
| Travel compatibility | — | — | ✅ |
| Group voting | — | — | ✅ |
| Fairness-aware planning | — | — | ✅ |
| Adaptive Plan Rescue | — | Disruption features focus mainly on travel logistics | ✅ |

> The comparison reflects the product features we reviewed during our research and is intended to show TripSync's design focus rather than claim that competing products cannot evolve.

---

# 5. Technical Architecture & Feasibility

## 🛠️ Tech Stack

| Technology | Purpose | Why We Chose It | Expected Constraint |
|---|---|---|---|
| **React / Next.js** | Frontend | Component-based development and suitable for quickly building an interactive prototype | Team learning curve and development time |
| **Supabase** | Authentication & Database | Provides authentication and PostgreSQL database features with a suitable free tier for prototyping | Free-tier limits and backend configuration |
| **AI API** | Itinerary generation | Allows TripSync to convert group preferences and trip constraints into readable itinerary suggestions | API cost, rate limits and inconsistent AI output |
| **Google Maps API** | Location / map information | Helps display attractions and understand locations | API quotas and billing requirements |
| **Weather API** | Weather information | Can support future automatic weather-based Plan Rescue | API reliability and free-tier limits |
| **Vercel** | Hosting | Simple deployment for a Next.js application | Free-tier limitations |

> **TODO:** Replace technologies above if your team chooses a different final stack.

---

## 🏗️ Proposed System Architecture

```text
                     ┌───────────────────┐
                     │      Users        │
                     │ Traveller / Group │
                     └─────────┬─────────┘
                               │
                               ▼
                     ┌───────────────────┐
                     │     Frontend      │
                     │  React / Next.js  │
                     └─────────┬─────────┘
                               │
                               ▼
                     ┌───────────────────┐
                     │ Backend / Supabase│
                     ├───────────────────┤
                     │ Users             │
                     │ Trips             │
                     │ Preferences       │
                     │ Group Members     │
                     │ Votes             │
                     │ Budget            │
                     │ Itinerary         │
                     └─────────┬─────────┘
                               │
                  ┌────────────┴────────────┐
                  ▼                         ▼
          ┌───────────────┐        ┌─────────────────┐
          │ AI / Rules    │        │ External APIs   │
          │ Engine        │        │ Maps / Weather  │
          └───────────────┘        └─────────────────┘
