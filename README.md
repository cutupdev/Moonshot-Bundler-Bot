# Solana Volume Bot

## Prerequisites

- Node.js (v14 or later recommended)
- npm (comes with Node.js)
- One or multiple Solana wallets with SOL

## Installation

1. Clone the repository:
   git clone https://github.com/youngpriince/sol-moonshot-bundler.git
   cd sol-moonshot-bundler

2. Install dependencies:
   npm install

3. Create a `.env` file in the root directory and add your configuration:
   AMOUNT=0.001
   TOKEN_ADDRESS=your_token_address
   DELAY=2000
   SLIPPAGE=1
   PRIORITY_FEE=0.0005
   JITO=false
   RPC_URL=your_rpc_url
   THREADS=2

## Usage

Run the bot with:

`node index.js`

## Configuration

Adjust the settings in your `.env` file to customize the bot's behavior:

- AMOUNT: The amount of SOL to swap in each transaction
- TOKEN_ADDRESS: The address of the token you're trading
- DELAY: Delay between swap cycles (in milliseconds)
- SLIPPAGE: Maximum allowed slippage (in percentage)
- PRIORITY_FEE: Priority fee for transactions
- JITO: Set to "true" to use Jito for transaction processing
- RPC_URL: Your Solana RPC URL
- THREADS: Number of parallel threads to run

## API Usage and Fees

This bot uses the Solana Swap API from [SolanaTracker.io](https://docs.solanatracker.io).

**Note**: The Swap API charges a fee for usage:

- Standard fee: 0.5% on each successful transaction

## License
