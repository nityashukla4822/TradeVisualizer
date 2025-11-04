# Real-Time Order Book Visualizer

A high-performance, real-time stock order book visualizer built using **Next.js** and the **Binance WebSocket API**.  
This project demonstrates the ability to handle high-frequency live data, manage complex state efficiently, and maintain a smooth, non-blocking user interface — all essential for financial applications.

---

## Live Demo
**[View the Live App](https://trade-visualizer-self.vercel.app/)**

---

## Tech Stack

| Category | Technology | Purpose |
|-----------|-------------|----------|
| **Framework** | Next.js (React + TypeScript) | Fast development, modular architecture, built-in optimizations |
| **Language** | TypeScript | Type safety, autocompletion, and better maintainability |
| **State Management** | Zustand | Lightweight and highly performant for real-time updates |
| **Styling** | Tailwind CSS | Clean, modern, and responsive design system |
| **API Source** | Binance WebSocket API | Live market data for order books and trades |

---

## Project Objectives

The key objectives of this project were to:

1. Establish a live WebSocket connection to Binance API.  
2. Handle **aggregate trades** and **order book delta** data streams efficiently.  
3. Maintain a continuously updating and responsive order book UI.  
4. Display live trade updates with visual cues for buy/sell direction.  
5. Ensure smooth performance under high-frequency data flow.  
6. Follow best practices in React performance optimization and code modularity.

---

## Features

- **Real-Time Order Book**  
  Continuously updates bids and asks from the live WebSocket feed.

- **Recent Trades Component**  
  Displays the latest 50 trades with color-coded direction (green for buy, red for sell).

- **Cumulative Totals and Spread**  
  Calculates running totals and the live bid-ask spread between top orders.

- **Depth Visualization**  
  Each row’s background bar represents cumulative depth, creating a visual “depth chart” effect.

- **Optimized Performance**  
  Uses Zustand store and memoization (`useMemo`, `useCallback`) to prevent unnecessary re-renders.

- **Error Handling and Auto-Reconnect**  
  Automatically handles connection drops and attempts reconnection.

- **Professional and Responsive UI**  
  Built with Tailwind CSS for a clean layout that works across devices.

---

## Folder Structure

```text
trade-visualizer/
│
├── public/
│   ├── favicon.ico
│   └── vercel.svg
│
├── src/
│   ├── app/
│   │   ├── globals.css           # Global Tailwind styles
│   │   ├── layout.tsx            # Root layout for Next.js
│   │   └── page.tsx              # Main page component
│   │
│   ├── components/
│   │   ├── OrderBook.tsx         # Displays real-time bids/asks with depth visualization
│   │   ├── RecentTrades.tsx      # Displays recent trades in real time
│   │   └── Spread.tsx            # Shows current bid-ask spread
│   │
│   ├── hooks/
│   │   └── useBinanceSocket.ts   # Custom hook for WebSocket connection and message handling
│   │
│   ├── store/
│   │   └── orderBookStore.ts     # Zustand store for maintaining global state
│   │
│   └── utils/
│       └── format.ts             # Utility for formatting numbers and prices
│
├── .gitignore
├── package.json
├── README.md
├── tsconfig.json
└── tailwind.config.js
```
Getting Started
1. Clone the Repository
git clone https://github.com/your-username/TradeVisualizer.git
cd TradeVisualizer
2. Install Dependencies
npm install
3. Run the Development Server
npm run dev


Key Learnings -> 

Handling real-time WebSocket data streams efficiently in React.

Using Zustand for performant, global state updates in a high-frequency environment.

Implementing depth visualization for order book data.

Applying React optimization hooks like useMemo and useCallback to minimize re-renders.

Managing API resilience through error handling and reconnection strategies.

Designing responsive and professional UIs for fintech dashboards.



