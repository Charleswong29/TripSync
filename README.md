# 🌍 TripSync by VEGE LLAO²

**Find people. Plan together. Travel better.**

**Team Members:** Celine Hew Boon Ling, Kok Jia Hui, Siew Hoi Wei, Wong Chee Yong  
**Problem Statement:** Travel Planner  
**Video Presentation:**  
**Presentation Slides:**  

---

# 1. Project Overview

## ✈️ The Problem

Planning a trip becomes more difficult when multiple people are involved.

Travellers may have different budgets, interests, travel pace, food preferences, transportation preferences and must-visit places. This makes group decision-making difficult, and one person often ends up doing most of the planning.

Solo travellers may face another problem: they want to travel but do not have a suitable travel companion because their friends may be unavailable, have different budgets or prefer different travel styles.

Travel plans can also become unsuitable when circumstances change. Bad weather, delays, tiredness, attraction closures, budget changes or changes in group members may require the group to revise the itinerary.

TripSync focuses on three connected problems:

- **Finding suitable people to travel with**
- **Helping a group reach agreement fairly**
- **Adapting the plan when circumstances change**

---

## 💡 Our Solution

**TripSync** is an AI-powered group travel planner and travel teaming prototype.

The experience is built around:

> **Find → Agree → Plan → Adapt**

TripSync supports two main ways to start a trip:

### Open Trip

For users who want to meet compatible travel companions.

An Open Trip can include:

- Destination
- Trip dates
- Minimum and maximum budget
- Transport preference
- Maximum members
- Travel styles
- Preferred traveller types such as Students, Young Adults, Food Lovers or Budget Travellers

Open Trips are intended for public discovery.

### Private Group

For users who already know who they want to travel with.

Current private group options include:

- Friends
- Family
- Couple
- School / Club
- Company / Team

Private Groups use invitation-based planning rather than public discovery.

---

## Current Core Features

- 👥 Open Trip and Private Group creation
- 🔎 Public trip discovery
- 🧩 Travel compatibility / group matching concept
- 🎭 Travel Personality and group preference collection
- 👤 Friends and Travel Buddies invitation flow
- 🗳️ Activity voting with Must Go, Like, Neutral and Skip
- 📊 Voting progress
- ⚖️ Group Match and Fairness Meter
- 🤖 AI-generated activity suggestions
- 🤖 AI-generated final itinerary flow
- 🚨 Plan Rescue
- ❤️ People / Travel Buddies management
- 🧭 Five main app areas: Explore, My Trips, Plan, People and Profile

---

# 2. Product Logic

## 2.1 Open Trip vs Private Group

TripSync separates public travel discovery from private planning.

| **Mode** | **Purpose** | **Access** |
|---|---|---|
| **Open Trip** | Find compatible travel companions | Public discovery |
| **Friends** | Plan with friends | Private |
| **Family** | Plan with family | Private |
| **Couple** | Plan as two people | Private |
| **School / Club** | Plan for a class, club or society | Private |
| **Company / Team** | Plan an outing, team building trip or retreat | Private |

Open Trips are used when the user still needs travel companions.

Private Groups are used when the group already exists.

---

## 2.2 Trip Creation

The current prototype uses a multi-step trip creation flow.

### Step 1 — Who are you travelling with?

Users choose:

- Open Trip
- Friends
- Family
- Couple
- School / Club
- Company / Team

### Step 2 — Trip Details

The current interface supports trip information such as:

- Trip Name
- State / Region
- Destination
- Trip Dates
- One-day Trip option
- Minimum Budget
- Maximum Budget
- Transport Preference
- Maximum Members
- Travel Style

Travel Style options include:

- Chill
- Food
- Nature
- Shopping
- Photography
- Adventure
- Culture
- Relaxation
- Team Building

### Step 3 — Open Trip Matching or Private Invitations

For an **Open Trip**, users can select matching preferences such as:

- Students
- Young Adults
- Food Lovers
- Photographers
- Adventure Travellers
- Relaxed Travellers
- Budget Travellers

For a **Private Friends Trip**, the prototype includes an Invite People screen with:

- Friends
- Travel Buddies
- Search
- Selectable people

---

# 3. Current Planning Flow

The current TripSync planning concept follows this sequence:

> **Group Lobby → Travel Preferences → Group Profile → Generate Attractions → Vote Together → Voting Progress → Group Match → Generate Final Itinerary → Itinerary → Plan Rescue**

---

## 3.1 Group Lobby

The Group Lobby is the shared workspace for one trip.

It can display:

- Trip name
- Group member count
- Current members
- Compatibility information
- Planning status
- Invitation actions
- Start / continue planning actions

For a newly created group without additional members, the intended empty state is to invite people before continuing as a group.

---

## 3.2 Travel Personality & Trip Preferences

TripSync uses travel preferences to understand each traveller.

Current preference categories include:

- Travel Style
- Food
- Wake-up Time
- Interests
- Transport preference
- Budget-related preferences

The prototype also contains a Group Profile / Group Vibe screen that combines member preferences into shared interests, compromise points and an AI suggestion.

---

## 3.3 Generate Attractions

Before building the final itinerary, TripSync creates candidate attractions for the group to review.

The current prototype includes a Curated Attractions screen with example activities such as:

- Genting SkyWorlds
- Awana SkyWay
- Chin Swee Caves Temple
- Skytropolis Indoor Theme Park
- Genting Premium Outlets

This stage is separate from final itinerary generation.

---

## 3.4 Vote Together

Members review attractions and vote using:

- **Must Go**
- **Like**
- **Neutral**
- **Skip**

The voting interface shows:

- Attraction
- Estimated cost
- Estimated duration
- Tags
- Match score
- Voting progress

After a user finishes their ballot, the prototype includes a Voting Progress screen.

---

## 3.5 Group Match & Fairness

After voting, TripSync presents group-level results.

The Group Match screen currently includes:

- Overall group match
- Group preference distribution
- Individual representation / fairness
- AI insight

The Fairness Meter is designed to highlight when one traveller's preferences are less represented than the rest of the group.

---

## 3.6 Final Itinerary

TripSync uses a separate AI generation stage to build the final trip plan after the group decision process.

The itinerary interface can show:

- Trip duration
- Estimated plan cost
- Group match
- Day tabs
- Timeline
- Activities
- Estimated activity cost
- Activity match

This separates:

> **AI activity suggestion**

from:

> **AI final itinerary generation**

---

## 3.7 Plan Rescue

Plan Rescue is TripSync's main adaptive feature.

The prototype is designed around six common problems:

- 🌧️ Bad Weather
- ⏰ Running Late
- 💸 Over Budget
- 😴 Too Tired
- 🚫 Place Closed
- 👥 Group Changed

Instead of rebuilding the whole trip, TripSync focuses on the affected part of the plan and proposes an updated itinerary.

---

# 4. Main App Areas

TripSync currently uses five primary navigation areas.

## Explore

Used for:

- Discovering Open Trips
- Searching for trips
- Starting Open Trip discovery
- Creating a new trip

## My Trips

Used for trips the user has created or joined.

## Plan

Used for continuing the planning process for the selected trip.

## People

Used for travel-related contacts and relationships such as:

- Friends
- Travel Buddies
- Family
- Classmates
- Team Members / Colleagues

## Profile

Used for the current user's travel preferences and personal profile.

---

# 5. What Makes TripSync Different

## 🔎 Travel Teaming

TripSync is not only about deciding where to go.

It also supports the step before planning:

> **Who should I travel with?**

Open Trips give solo travellers and other users a way to discover compatible travel groups.

---

## ⚖️ Group Fairness

Normal majority voting can repeatedly favour the same people.

TripSync therefore includes a Fairness Meter to make underrepresented preferences visible during group planning.

---

## 🚨 Plan Rescue

TripSync is designed to remain useful after the itinerary has already been created.

Instead of starting again when something changes, Plan Rescue focuses on repairing the affected section of the trip.

---

## 🎮 Game-Like Group Formation

TripSync takes inspiration from multiplayer team formation.

Instead of:

> **Find players → Form team → Play**

TripSync uses:

> **Find travellers → Form group → Agree → Travel**

---

# 6. Ideation & Idea Evolution

## 6.1 Initial Mind Map

At the beginning of our ideation process, our team explored different problems and possible features related to group travel planning.

The mind map helped us explore several areas, including:

- Travel Teaming
- User Experience
- Travel Experience
- Planning & Itinerary
- Budget & Expenses
- Plan Rescue and Adaptation

<img width="820" height="453" alt="photo_2026-09-11_21-09-19" src="https://github.com/user-attachments/assets/8aa2f0d7-4971-40a5-8a22-9b0565d3bdb2" />


## 6.2 Idea Evolution

<img width="820" height="453" alt="photo_2026-09-11_20-51-45" src="https://github.com/user-attachments/assets/dd45aebb-cfbc-4ee2-9fb4-d3caefb46358" />

## Version 1 — AI Travel Planner

The first idea focused mainly on generating an itinerary from destination, budget and preferences.

---

## Version 2 — Group Travel Planner

The concept expanded to include:

- Group preferences
- Voting
- Group matching

---

## Version 3 — Adaptive Group Travel Planner

TripSync added:

- Fairness Meter
- Plan Rescue
- Adaptive planning

---

## Version 4 — Travel Teaming + Group Planning

The concept expanded again with:

- Open Trips
- Private Groups
- Travel compatibility
- Travel Buddies
- School / Club Trips
- Company / Team Trips

This led to the current positioning:

> **Find people. Plan together. Travel better.**


## 6.3 User Flow

<img width="840" height="440" alt="photo_2026-09-11_21-01-16" src="https://github.com/user-attachments/assets/0bd4c56b-c03e-4f8b-8756-39e3219143d7" />

---

# 7. Prototype

**UI Prototype:**  
[https://ai.studio/apps/afdaea94-28d1-468e-a89f-609de2f72771](https://ai.studio/apps/afdaea94-28d1-468e-a89f-609de2f72771)

The current prototype demonstrates the main TripSync product structure and planning flow.

Features still being refined in the current implementation include:

- Trip-specific routing
- Invitation handling
- Owner / visitor actions
- Editing created trips
- Shared multi-user state
- Some dynamic data binding

The README therefore describes the current implemented prototype direction without treating unfinished or unverified integrations as completed features.

---

# 8. Future Development

Features intentionally left outside the current prototype include:

- Live weather integration
- Advanced route optimisation
- Hotel / flight / bus booking
- Payment processing
- Travel marketplace
- Merchant offers and partnerships
- Full social media / chat system

These are future extensions rather than requirements for the current TripSync MVP.

---

# Final Product Story

TripSync is not only an AI itinerary generator.

Its core experience connects:

> **Find people → Build a group → Understand preferences → Vote together → Create a fair plan → Adapt when plans change**

## **Find people. Plan together. Travel better.**
