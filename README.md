# Stock Portfolio Platform - Rajsi Traders

This project is a backend implementation for Rajsi Traders' Stock Portfolio Platform. It allows users to add stocks to their portfolio, calculate returns, and view the status of their investments.

## Features

1. **Calculate Returns**: Calculate the return value for a single stock.
2. **Total Returns**: Calculate the total return value for all stocks in the portfolio.
3. **Return Percentage**: Calculate the return percentage for a single stock.
4. **Total Return Percentage**: Calculate the total return percentage for all stocks in the portfolio.
5. **Stock Status**: Determine if a stock is in profit or loss based on the return percentage.

## API Endpoints

1. **Calculate Returns**
   - Endpoint: `/calculate-returns`
   - Parameters: `boughtAt`, `marketPrice`, `quantity`
   - Example: `http://localhost:3000/calculate-returns?boughtAt=300&marketPrice=400&quantity=2`
   - Output: `200`

2. **Total Returns**
   - Endpoint: `/total-returns`
   - Parameters: `stock1`, `stock2`, `stock3`, `stock4`
   - Example: `http://localhost:3000/total-returns?stock1=100&stock2=200&stock3=200&stock4=400`
   - Output: `900`

3. **Return Percentage**
   - Endpoint: `/calculate-return-percentage`
   - Parameters: `boughtAt`, `returns`
   - Example: `http://localhost:3000/calculate-return-percentage?boughtAt=400&returns=200`
   - Output: `50`

4. **Total Return Percentage**
   - Endpoint: `/total-return-percentage`
   - Parameters: `stock1`, `stock2`, `stock3`, `stock4`
   - Example: `http://localhost:3000/total-return-percentage?stock1=10&stock2=20&stock3=20&stock4=40`
   - Output: `90`

5. **Stock Status**
   - Endpoint: `/status`
   - Parameters: `returnPercentage`
   - Example: `http://localhost:3000/status?returnPercentage=90`
   - Output: `profit`

## How to Run

1. Clone the repository.
2. Install dependencies: `npm install`.
3. Start the server: `node app.js`.
4. Access the APIs at `http://localhost:3000`.

## Frontend Integration

The backend APIs are designed to be integrated with Rajsi Traders' frontend UI. Update the API URLs in the frontend code to point to the deployed backend.

## Live Demo

Check out the live demo of the frontend: [Rajsi Traders Stock Platform](https://bd1-stocks.vercel.app/).

---

Developed by Divyanshu Jadaun for Rajsi Traders.
