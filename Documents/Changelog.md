
Here is an initial changelog for the bot, covering the main features and changes in this version:

Changelog
Version 1.0.0 – Initial Release
Release Date: YYYY-MM-DD

Features:
Discord Integration:

The bot connects to Discord and allows users to interact with it via slash commands.
Slash commands include /dashboard, /trade, /balance, /history, and others to manage and monitor trades.
Trading Functionality:

Supports buying and selling tokens (WVTRU/USDC) using Ethers.js.
Automatic trading functionality based on predefined buy and sell conditions.
Ability to execute limit orders with an adjustable fee percentage (currently set to 2%).
Manual trading available through the /trade command for free, while limit orders incur a 2% fee.
Trading logic uses the Vitruveo network for swaps and price calculations.
Automated Trading System:

Automatic trading based on price thresholds and percentage changes.
Ability to pre-set buy and sell conditions based on price movements or percentage changes.
The bot automatically monitors and executes trades if conditions are met.
Limit Orders:

Place limit buy or sell orders to be triggered when a certain price is reached.
Cancel active limit orders using the /cancel-limit-order command.
View active limit orders using /list-limit-orders.
Token Balances:

Check wallet balances for USDC and WVTRU using the /balance command.
Fetch native token (ETH/VTRU) balance as well.
Transaction History:

Fetch and view recent buy and sell transaction history via the /history command.
Transactions are stored in JSON files for persistence.
Customizable Trade Settings:

Adjustable TRADE_INTERVAL for setting trade frequency in milliseconds (default 15 seconds).
Easily set buy and sell percentages using environment variables.
Price Chart Generation:

Generate price charts using QuickChart and display them in the dashboard.
Pre-Approval Mechanism:

The bot pre-approves the necessary tokens for trading, reducing manual interaction.
Slash Commands:
/dashboard: Displays a trading dashboard with price information, active conditions, and limit orders.
/trade: Manually buy or sell a specific amount of WVTRU.
/balance: Shows the current balance of USDC, WVTRU, and the native currency.
/history: Displays the recent buy and sell transactions for WVTRU.
/set-trade-interval: Adjusts the trade interval for automatic trades.
/add-buy-condition and /add-sell-condition: Add buy or sell conditions based on percentage or price.
/remove-buy-condition and /remove-sell-condition: Remove existing buy or sell conditions by ID.
/place-limit-order: Place a limit buy or sell order.
/cancel-limit-order: Cancel an active limit order by its ID.
/list-limit-orders: View all active limit orders.
Security and Safety:
Recommended creating a new wallet specifically for the bot's use to minimize risks.
Private key safety is highlighted with reminders to secure wallet details.
No liability for any potential losses, outlined in the disclaimer.
