# Real-Time Order Book Visualizer

A high-performance, real-time stock order book visualizer built using **Next.js** and the **Binance WebSocket API**.  
This project demonstrates the ability to handle high-frequency live data, manage state efficiently, and maintain a smooth, non-blocking user interface — all critical for modern financial systems.

---

## Live Demo
**[View the Live App](https://trade-visualizer-self.vercel.app/)**

---

## Tech Stack

| Category | Technology | Purpose |
|-----------|-------------|----------|
| **Framework** | Next.js (React + TypeScript) | High performance, modular architecture, and built-in SSR |
| **Language** | TypeScript | Type safety and better developer experience |
| **State Management** | Zustand | Lightweight and fast, ideal for real-time updates |
| **Styling** | Tailwind CSS | Clean, responsive, and maintainable design system |
| **API Source** | Binance WebSocket API | Provides continuous real-time order book and trade data |

---

## Project Objectives

The primary objectives of this project were to:

1. Connect to Binance WebSocket streams and subscribe to live market data.  
2. Render real-time order book updates with bid/ask depth aggregation.  
3. Display recent trades in a continuously updating table.  
4. Optimize UI rendering to avoid frame drops during high-frequency updates.  
5. Maintain clean modular code and reusable components.

---

## Features

- **Real-Time Order Book Updates**  
  Live bid and ask prices update dynamically as new data arrives.

- **Recent Trades Feed**  
  Displays the latest trades, differentiating between buy and sell orders.

- **Efficient State Management**  
  Uses Zustand for minimal re-renders and optimized performance under load.

- **Responsive and Minimal UI**  
  Built with Tailwind CSS for a clean, modern, and adaptive layout.

- **Error Handling and Auto-Reconnect**  
  Handles WebSocket disconnections gracefully and auto-reconnects when required.

---

## Folder Structure

