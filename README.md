#### Welcome to the iData Research Web Developer Test

##### Keep it clean and simple

##### The test should take approximately 1 hour

=========================================================

System Requirements:

- Node.js
- Npm

Note: You need Node.js/npm to run the project -- but you do not need to do work in the backend unless you chose to.
Note: See below for some useful links

1. Your goal is to create a simple interface that looks similar to this:

   ![image](./screenshots/Snapshot.PNG)

2. Fork the repository, clone and create a branch under test/[Your First Name]

3. This repository uses Node.js, and includes bootstrap and axios -- you must install dependencies and run the server first (run *node index.js*)

4. When you are done, push your **branch**, and submit a pull request.

User stories:

1. The user will click on a 'Submit' button, and it will generate a table with simple data from Yahoo Finance API. The table will consist of:
   a. Time stamp of current date and time -- not 'Regular Market Time'
   b. Currency (USD)
   c. Symbol
   d. Regular Market Price

All you need to do is make an API call to: `~/api`. API keys, and actual URL is done within the backend to keep things quick and simple. the Node.js backend should return this data:

Note: that all you need is `chart / result / meta` in order to access the required data.

```
{
    "chart": {
        "result": [
            {
                "meta": {
                    "currency": "USD",
                    "symbol": "AAPL",
                    "exchangeName": "NMS",
                    "instrumentType": "EQUITY",
                    "firstTradeDate": 345479400,
                    "regularMarketTime": 1591985129,
                    "gmtoffset": -14400,
                    "timezone": "EDT",
                    "exchangeTimezoneName": "America/New_York",
                    "regularMarketPrice": 335.47,
                    "chartPreviousClose": 335.9,
                    "previousClose": 335.9,
                    "scale": 3,
                    "priceHint": 2,
                    ....
```

Links:
- [Git Commands](https://about.gitlab.com/images/press/git-cheat-sheet.pdf)
- [Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch) and [Axios](https://github.com/axios/axios/blob/master/README.md)
- [Bootstrap](https://getbootstrap.com/docs/4.5/getting-started/introduction/)
