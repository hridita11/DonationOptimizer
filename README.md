## DonationOptimizer
a web platform where a user inputs a donation amount, and the system finds GoFundMe campaigns that their donation would meaningfully complete or push to a milestone.


# Flow:
1. User enters a donation amount (e.g., $50).
2. The system queries your campaign database (regularly updated from GoFundMe and others).
3. Finds campaigns close to their goals or with time urgency.
4. Displays a few top suggestions with transparency and links (“Your $50 will complete this goal”).
5.  user either donates directly through GoFundMe or through your site as a connector.

# Tech Stack Overview

Layer	Tech:	Purpose
Backend API:	Python + FastAPI -	Handle users’ donation input, run matching logic
Database:	SQLite-Store fetched GoFundMe campaign data
Data fetch:	Python scraper / static dataset	- Pull campaign info periodically
Frontend:	Next.js / React	User-facing donation interface
Hosting: Render	Deploy app easily


# Challenges:

GoFundMe does not offer a public API anymore
