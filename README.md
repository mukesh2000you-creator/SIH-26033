# Smart India Hackathon Workshop
# Date:24/11/26
## Reference Number:26019585
## Name:Mukesh Manohar 

## Problem Title
CROPBRIDGE AI:AI-Powered Agricultural Price Discovery and Direct Buyer Connection Platform

## Problem Creater's Organization
Ministry of Consumer Affairs, Food & Public Distribution

## Theme
Agriculture, FoodTech & Rural Development

## Problem Description
Expected Solution: Create a digital marketplace that:

• Connects farmers/FPOs directly with consumers and bulk buyers.
• Provides logistics support.
• Uses AI for demand forecasting and route optimization.

Benefits:

• Better prices for farmers.
• Lower prices for consumers.
• Reduced supply chain inefficiencies.

## Proposed Solution
CropBridge AI is an AI-powered agricultural price discovery and direct buyer connection platform designed to help
farmers identify profitable selling opportunities. It connects farmers directly with retailers, supermarkets, restaurants,
wholesale buyers and food-processing businesses.
The platform addresses low farmer earnings and high consumer prices caused in part by multiple intermediaries,
limited price transparency, fragmented buyer access and transportation costs. Rather than showing only the highest
quoted price, CropBridge AI compares buyer offers and estimates the farmer’s net earnings after transportation and
other expenses.
## How the solution works
1. Farmers register and list their crops, available quantity, quality, harvest date and farm location.
2. Buyers register and publish their requirements, including crop type, quantity and expected delivery details.
3. The system matches crop listings with suitable buyer requirements based on crop, quantity and location.
4. The platform compares available buyer offers and estimates net earnings after transport and other estimated
   costs.
5. Farmers review the comparison and contact the buyer they choose. The platform supports informed decisions; it
   does not guarantee a sale or a particular price.
## Key features
• Farmer registration and crop listing
• Buyer registration and purchase requirements
• Crop-, quantity- and location-based buyer matching
• Buyer-offer and market-price comparison
• Net earnings estimator
• Transportation cost estimator
• Farmer dashboard and enquiry status
## Proposed innovation: Net Profit Recommendation Engine
The recommendation engine ranks suitable buyer options using estimated net earnings rather than purchase price
alone. A simple initial implementation can use transparent rule-based calculations. Machine-learning-based price
prediction can be considered later when sufficient reliable historical data is available.
Estimated net earnings = (Quantity × Buyer offer per unit) − Estimated transportation cost − Other estimated
expenses.
## Illustrative example
For 1,000 kg of tomatoes, a buyer offering 20/kg may appear best. If estimated transportation and other costs are
2,000, the estimated net earnings are 18,000. A different buyer offering 18/kg with 1,000 in estimated costs
would provide 17,000. These figures are illustrative only; actual offers, quality, quantity acceptance and costs must
be confirmed.

## Technical Approach
Application workflow
The farmer or buyer accesses the web application and registers. Farmers create crop listings, while buyers publish
purchase requirements. The Flask backend stores and retrieves records from SQLite, matches compatible listings
and requirements, and sends relevant offer data to the recommendation engine. The engine compares offers and
estimated costs, then presents ranked options and calculations on the farmer dashboard.
<img width="773" height="450" alt="Screenshot 2026-11-24 222634" src="https://github.com/user-attachments/assets/cfb1b759-cfb4-4d13-8611-e8696e254a28" />

## Technology stack
• Frontend: HTML, CSS and JavaScript for responsive pages, forms and dashboards.
• Backend: Python with Flask for authentication, application routes, listing management and matching logic.
• Database: SQLite for prototype storage of users, crop listings, buyer requirements and enquiries.
• Data analysis: Python calculations with Pandas and NumPy where useful.
• Optional machine learning: Scikit-learn Linear Regression for an experimental price-trend estimate, only if
sufficient suitable historical data is available.
## Core processing steps
1. Validate farmer crop listings and buyer requirements.
1. Filter buyers by crop compatibility, quantity and location.
1. Calculate estimated revenue and costs for each suitable buyer.
1. Rank options by estimated net earnings and show the assumptions used.
1. Allow the farmer to review details and contact the selected buyer.
##Data approach
The first prototype can use clearly labelled sample data and manually entered buyer offers. AGMARKNET and
e-NAM may be explored as potential sources or references for agricultural market information. Any integration must
follow the relevant site's access conditions, data availability and update frequency. The application should display the
source and date of any market-price data it presents.
## Prototype scope
The first version focuses on registration, crop listings, buyer requirements, matching, offer comparison, cost
estimation and a farmer dashboard. Advanced forecasting, live logistics integration, payments and large-scale
deployment are future enhancements rather than required prototype features.

## Feasibility and Viability
Technical feasibility:-
• The proposed frontend and backend technologies are widely used and suitable for a student prototype.
• Flask and SQLite keep the initial architecture lightweight and manageable.
• Buyer matching and net earnings ranking can be implemented with basic filtering and arithmetic before introducing
machine learning.
• The prototype can run on an ordinary laptop and be demonstrated with sample farmer, crop and buyer records.
Economic feasibility:-
• The core development stack is free or open source.
• A prototype can be built without dedicated servers or costly hardware.
• Initial testing can use a small, controlled dataset and a limited pilot group.
Operational feasibility:-
• Farmers can enter crop details through a simple mobile-friendly interface.
• Buyers can post requirements and review relevant listings.
• The system provides comparisons and estimates while leaving the final selling decision with the farmer.
<img width="800" height="367" alt="image" src="https://github.com/user-attachments/assets/ce85b88d-e6c7-407a-ad59-4d305ad1114a" />
Overall viability: CropBridge AI is suitable for a low-cost prototype and can be expanded in stages. Its practical value
should be assessed through a pilot that measures successful buyer connections, accuracy of cost estimates, user
experience and changes in realized farmer earnings. The platform cannot guarantee higher prices or eliminate
intermediaries on its own

## Impact and Benefits
Farmers:-
• Improves access to multiple potential buyers and their offers.
• Makes it easier to compare estimated net earnings rather than headline prices alone.
• Provides a structured way to share crop availability and receive enquiries.
• May reduce dependence on a single buyer or intermediary where alternative buyers are available.
Consumers:-
• More direct sourcing may create opportunities to reduce avoidable distribution costs.
• Improved supply-chain visibility may support more informed purchasing.
Retailers, restaurants and other buyers
• Makes it easier to discover farmers offering required crops and quantities.
• Can reduce the effort involved in identifying local suppliers.
• Provides a clearer process for submitting requirements and purchase enquiries.
Agricultural supply chain:-
• Encourages price comparison and more transparent buyer-seller communication.
• Can support better planning of procurement and transportation.
• Creates a digital record of listings and enquiries for follow-up.
Potential wider benefits:-
• Social: supports access to market information and digital services.
• Economic: may improve selling decisions and reduce avoidable procurement costs.
• Technological: demonstrates practical use of data analysis and AI-assisted recommendations.
• Environmental: better coordination may reduce unnecessary trips, subject to actual logistics planning.
These are expected or potential benefits, not proven outcomes. Their scale will depend on adoption, data quality,
buyer participation, transport availability and local market conditions.
Future expansion:-
• Support additional crops, districts and market regions.
• Add regional-language interfaces and assisted onboarding.
• Integrate verified agricultural price data where access is permitted.
• Explore demand forecasting after collecting adequate historical data.
• Support Farmer Producer Organizations (FPOs) and group listings.
• Integrate transport providers and delivery status tools.


## Research and References
https://enam.gov.in/
https://agmarknet.gov.in/
https://www.pib.gov.in/PressReleasePage.aspx?PRID=2050966
https://agritechobservatory.review.fao.org/en/digital-technology-and-agricultural-markets
