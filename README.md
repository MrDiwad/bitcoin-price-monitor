# Bitcoin Price Monitor (n8n)

# What is this? 
A simple automation that keeps an eye on the bitcoin. It tracks price changes and alerts only when something interesting is happening (like a significant "dip").

# How it works:

Schedule: The workflow runs automatically every hour.

Data Fetch: It pulls real-time data for Bitcoin directly from the CoinGecko API using an HTTP Request.

Smart Logic: Instead of just reporting the price, it checks the 24h percentage change.

Conditional Alert: If the price drops by more than 4% or goes up by 4%, it triggers an action.

Notification: It sends a formatted alert to Discord, letting know it might be a good time to "buy the dip." or open short position.

# Tech stack:

n8n (Self-hosted via Docker)

CoinGecko Public API (No API keys required for this version)

Discord Webhooks

JSON & Logic Routing

<img width="2275" height="1175" alt="image" src="https://github.com/user-attachments/assets/544b156a-bf2d-4d32-95b3-9ba9f7090d87" />
