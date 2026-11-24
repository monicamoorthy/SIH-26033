# Smart India Hackathon Workshop
## Date: 24.11.2026 
## Reference Number: 26013095
## Name: Monica M<br><br>

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.<br><br>

## Problem Creater's Organization
Ministry of Consumer Affairs, Food & Public Distribution<br><br>

## Theme
Agriculture, FoodTech & Rural Development<br><br>

## Problem Description
Expected Solution: Create a digital marketplace that:<br><br>

• Connects farmers/FPOs directly with consumers and bulk buyers.<br>
• Provides logistics support.<br>
• Uses AI for demand forecasting and route optimization.<br>

Benefits:
<br><br>
• Better prices for farmers.<br>
• Lower prices for consumers.<br>
• Reduced supply chain inefficiencies.<br><br>

## Proposed Solution<br>
We are building **KrishiSetu**, a direct farm-to-fork digital marketplace that connects farmers and Farmer Producer Organizations (FPOs) directly with households, retailers, and bulk buyers. 

* **How it addresses the problem:** By eliminating unnecessary middlemen (commission agents and layered wholesalers), farmers list their harvest directly at transparent prices while buyers purchase fresher produce closer to farm-gate rates.<br>
* **Key Features & Innovation:** 
  * **Voice-First & Multilingual Interface:** Farmers can list crops using simple voice notes in regional languages, removing literacy barriers.<br>
  * **Smart Order Pooling:** Aggregates small orders from nearby consumers or restaurants into single bulk pickups to keep transport affordable.<br>
  * **Escrow & Instant UPI Settlement:** Funds are held securely upon order placement and released to the farmer immediately upon pickup verification.<br><br>
  
## Technical Approach<br>
**Frontend:** React Native (cross-platform mobile app for farmers and delivery partners) and Next.js (web dashboard for bulk buyers and FPO admins).<br>
* **Backend & Database:** Node.js with Express, PostgreSQL for transactional data, and Redis for real-time inventory locking.<br>
* **AI & Optimization:** Python (FastAPI) running Prophet/XGBoost models for regional crop demand forecasting and Google OR-Tools for dynamic vehicle routing (VRP).<br>
* **Integrations:** Razorpay Route / UPI for split payments, Bhashini API for Indian regional voice-to-text, and OpenStreetMap / Google Maps APIs for live tracking.<br><br>
* **Implementation Process:**<br>
  1. **Onboarding:** FPOs and farmers register via Aadhaar/phone OTP and list available harvest with quality grades.
  2. **Demand Matching:** AI predicts weekly urban demand and suggests optimal harvest quantities and fair dynamic pricing.
  3. **Dispatch & Delivery:** Orders are clustered by proximity, assigned to verified local mini-trucks/logistics partners via optimized routes, and tracked until doorstep delivery.<br><br>
     <img width="1024" height="572" alt="dd6044b4-8782-4afe-abfa-863a07968f58" src="https://github.com/user-attachments/assets/773aba71-2628-41e8-8568-8c8b6e2544b6" />
</b><br><br>

## Feasibility and Viability<br>
* **Feasibility:** High. Smartphone and UPI penetration in rural India—paired with existing FPO networks—allows rapid onboarding without heavy hardware investments.<br>
* **Potential Challenges & Risks:**<br>
  * Low digital literacy among small-scale farmers.<br>
  * Spoilage of perishable produce during transit.<br>
  * Trust deficit regarding quality grading and payment delays.<br>
* **Mitigation Strategies:**<br>
  * Partner with local FPOs to act as physical collection and quality-check hubs.<br>
  * Use AI route optimization to minimize transit time and prioritize cold-chain vehicles for high-perishable crops.<br>
  * Automate instant UPI payouts upon handover to build immediate financial trust.<br><br>

## Impact and Benefits<br>
* **Economic Impact:** Increases farmer profit margins by **20%–35%** by capturing middleman markups, while lowering retail prices for consumers by **10%–20%**.<br>
* **Social Impact:** Empowers rural farming communities with price transparency, predictable demand, and financial independence.<br>
* **Environmental Impact:** Reduces food wastage caused by multi-stage handling and cuts carbon emissions through consolidated, route-optimized delivery trips.<br><br>

## Research and References<br>
* **e-NAM (National Agriculture Market):** [enam.gov.in](https://www.enam.gov.in/) — Studied existing digital mandi workflows and gaps in last-mile logistics.<br>
* **SFAC (Small Farmers' Agribusiness Consortium):** [sfacindia.com](http://sfacindia.com/) — Referenced FPO aggregation models for small and marginal farmers.<br>
* **ONDC (Open Network for Digital Commerce):** [ondc.org](https://ondc.org/) — Explored open-network protocols for hyperlocal logistics and seller discovery.<br>
* **FAO Food Loss & Waste Reports:** [fao.org](https://www.fao.org/platform-food-loss-waste/) — Benchmarked post-harvest supply chain inefficiencies in perishable produce.
