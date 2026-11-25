# Smart India Hackathon Workshop

# Date: 23-11-2026

## Reference Number: 26014806

## Name: JEROFIN RENNET J

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers' earnings and increase consumer prices.

## Problem Creator's Organization
Ministry of Consumer Affairs, Food & Public Distribution

## Theme
Agriculture, FoodTech & Rural Development

## Problem Description
**Expected Solution:** Create a digital marketplace that:
- Connects farmers/FPOs directly with consumers and bulk buyers.
- Provides logistics support.
- Uses AI for demand forecasting and route optimization.

**Benefits:**
- Better prices for farmers.
- Lower prices for consumers.
- Reduced supply chain inefficiencies.

## Proposed Solution

### 1. Detailed explanation of the proposed solution
**KisanHub** is a mobile and web marketplace where consumers order fresh produce directly from farmers and FPOs, in the familiar style of quick-commerce apps. Existing ration (fair price) shops act as local "Kisan Hubs" for collection, storage, and handover, so no new last-mile network is needed.

**How it works:**
- Farmers and FPOs list produce, quantity, grade photos, and price.
- Consumers pre-order for a chosen delivery slot.
- AI forecasts demand for each shop area and tells farmers what to bring.
- Farmers' produce is pooled, and an optimized route delivers it to several hubs.
- The shop checks quality on arrival.
- Consumers pick up at the shop or choose home delivery.
- Payment is released to the farmer after handover.

**Key features:**
- **Pre-order, harvest-to-order model:** Farmers harvest only what is ordered, which reduces wastage.
- **Ration shop as Kisan Hub:** The owner earns a small fixed commission per order.
- **FPO and village aggregation:** Several farmers' produce is pooled into shared loads.
- **Two delivery options:** Pickup at the shop (free or very cheap), or home delivery for a small fee by local partners such as women self-help group members.
- **Ration card integration:** Easy onboarding, with scope for subsidy or wallet features later.
- **Rural accessibility:** Regional-language and voice interface, SMS/WhatsApp ordering, and a shop-assisted order desk for people without smartphones.
- **Price transparency:** The farmer's price, hub commission, and delivery fee are shown separately, with a comparison to the local market price.
- **Quality assurance:** Photo grading at listing, a check at the hub, ratings, and easy refunds.
- **Surplus clearance:** Near-expiry produce is sold at a discount.
- **Cold-chain add-on (phase 2):** Small solar-powered cold boxes at larger hubs for perishables.

### 2. How it addresses the problem
- The chain shrinks to **Farmer → Ration Shop → Consumer**, with no agents, traders, or wholesalers in between.
- The only added charges are a small delivery fee and a small hub commission.
- Existing shops remove the need for new infrastructure.
- Pooled, route-optimized deliveries cut transport cost per kg.
- Pre-orders and AI forecasting reduce wastage and price swings.

### 3. Innovation and uniqueness
- It uses ration shop infrastructure as the last-mile network, which existing apps don't do.
- It combines pre-order demand forecasting with pooled, route-optimized farmer deliveries.
- It works for low-literacy and low-connectivity users through voice, regional languages, and shop-assisted ordering.
- Pricing is fully transparent.
- Hub owners and self-help groups earn income, so the model is inclusive.

## Technical Approach

### 1. Technologies to be used

| Layer | Technology |
| --- | --- |
| Frontend | React / React Native (PWA for low-end phones) |
| Backend | Python (Django/FastAPI) or Node.js |
| Database | PostgreSQL with PostGIS, Redis for caching |
| AI/ML | Python, scikit-learn, Prophet/XGBoost for demand forecasting |
| Route optimization | Google OR-Tools (vehicle routing), OpenStreetMap/Google Maps API |
| Image grading | Basic computer vision on listing photos (phase 2) |
| Payments | UPI/Razorpay with escrow-style release |
| Language and voice | Bhashini/Google APIs for translation and speech |
| Messaging | SMS/WhatsApp APIs |
| Hosting | AWS/GCP, Docker |

### 2. Methodology and process for implementation
<img width="1213" height="1297" alt="image" src="https://github.com/user-attachments/assets/6dd5974b-7a47-460d-a6f1-061aebf818ae" />


## Feasibility and Viability

### 1. Analysis of feasibility
- The technology is mature and widely available.
- Ration shops, UPI, and government data ([eNAM](https://enam.gov.in), [Agmarknet](https://agmarknet.gov.in)) already exist.
- Revenue comes from a small platform fee, a hub commission, and a delivery margin.
- A pilot in a few districts is realistic.

### 2. Potential challenges and risks
- Ration shops are licensed and government-regulated, so partnership approval is needed.
- Perishables need cold storage.
- Rural digital literacy and connectivity are limited.
- Farmer logistics can be costly for small loads.
- Shop owners need an incentive to join.
- Quality consistency and trust.
- Cold start: too few buyers or farmers at the beginning.

### 3. Strategies for overcoming these challenges
- Start with a pilot with a state civil supplies department or willing shop owners.
- Begin with non-perishable and semi-perishable crops, then add cold boxes.
- Use voice and vernacular interfaces and the shop-assisted order desk.
- Aggregate through FPOs and use route optimization.
- Pay hub owners a fixed commission per order.
- Use photo grading, ratings, and refunds.
- Launch in a few villages and a few crops, with bulk buyers first to guarantee demand.

## Impact and Benefits

### 1. Potential impact on the target audience
- **Farmers/FPOs:** Higher earnings, guaranteed demand, and faster payment.
- **Consumers:** Fresher produce at lower, transparent prices.
- **Delivery partners (including SHG women):** Local employment.

### 2. Benefits of the solution
- **Economic:** Higher farmer income, lower retail prices, lower transaction costs.
- **Social:** Rural livelihoods, women's participation, digital inclusion.
- **Environmental:** Less food waste, fewer empty trips, and lower emissions through pooled routes.

## Research and References
- **eNAM:** https://enam.gov.in
- **Agmarknet (mandi prices):** https://agmarknet.gov.in
- **ONDC:** https://ondc.org
- **SFAC (FPO promotion):** https://sfacindia.com
- **Google OR-Tools routing:** https://developers.google.com/optimization/routing
- **SIH portal:** https://sih.gov.in
- **Public Distribution System and fair price shop details:** Cite your pilot state's civil supplies department website.









