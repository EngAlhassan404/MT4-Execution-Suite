# MT4 Execution Suite
![Version](https://img.shields.io/badge/Version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Author](https://img.shields.io/badge/Author-Eng.%20Alhassan%20Ali%20Mubarak%20Bahbah-purple.svg)

A professional, high-performance toolkit designed for the manual trader on the MetaTrader 4 platform. This suite was built with a single goal: to bridge the gap between limited manual execution and full automation, providing a level of speed and precision that surpasses human capabilities.

## The Project's Philosophy

The philosophy of this suite is to act as **"The Programmatic Finger"** for the trader. In the world of trading, especially in high-stakes competitions where maximizing returns is the ultimate goal, a decisive moment is everything. These tools do not make decisions for you; they execute your decisions with maximum velocity and scale, turning tasks that would take minutes to perform manually into operations that are completed in a fraction of a second.

---
## The Problem: Limitations of Manual Trading & MT4

This suite was engineered to overcome two major obstacles that every active trader faces:

1.  **Drawbacks of Manual Execution:**
    * **Extremely Slow:** Manually opening or closing 10 trades can take over a minute—long enough to miss the optimal entry or exit price.
    * **Prone to Errors:** An increased number of clicks raises the probability of mistakes, such as entering the wrong lot size or forgetting a stop loss.
    * **Mental Pressure:** Under volatile market conditions, rapid manual execution becomes a stressful mental task.

2.  **Shortcomings of the MetaTrader 4 Platform:**
    * **No Native Bulk Operations:** The platform lacks built-in functions to open or close all trades with a single click, forcing a tedious one-by-one workflow.
    * **Limited Analysis Tools:** MT4 does not provide a quick way to count open positions based on specific filters (e.g., by profit or loss).

---
## The Solution: The MT4 Execution Suite Tools

This suite offers an integrated solution to these problems through four highly efficient tools:

### 1. The Opener Script (MT4_Execution_Suite_Opener.mq4)
The primary execution tool for opening a large number of trades with a single click.

**Performance Report (Successful Execution Example):**
![Opener Performance](Documentation/MT4_Execution_Suite_Opener.png)
This image shows the performance report after successfully executing **100 Sell trades**. The report displays all vital statistics, including the first and last trade prices, the average entry price, and the price drift.

* **Execution Speed Analysis:**
    * **Total Time:** 100 trades were opened in just **30.78 seconds**.
    * **Performance Rate:** An execution rate of up to **3.25 trades per second** (or ~195 trades per minute).

**Intelligent Reporting & Safety Feature (Partial Execution Example):**
![Opener Stop Reason](Documentation/MT4_Execution_Suite_Opener_Stop_Reason.png)
This image demonstrates the script's most critical feature: **intelligent reporting**. Here, the script attempted to open 100 trades but automatically stopped after opening only **14**. The report explicitly states the **Stop Reason**: the free margin reached the safety limit defined in the settings. This feature protects the user from excessive risk and provides full transparency.


### 2. The Counter Script (MT4_Execution_Suite_Counter.mq4)
A monitoring tool for accurately analyzing the account's current state using advanced filters.

![Counter Performance](Documentation/MT4_Execution_Suite_Counter.png)
This image showcases the Counter script's ability to analyze open positions. In this example, the combined filters were used to count **all open trades** (Buys & Sells, Profitable & Losing) for the EURUSD symbol, resulting in a total of **100 trades**. This tool is perfect for getting a quick and precise overview of total market exposure.

### 3. The Closer Script (MT4_Execution_Suite_Closer.mq4)
A powerful tool for closing trades in bulk based on specific rules (close all, profitable only, losing only, etc.).

![Closer Performance](Documentation/MT4_Execution_Suite_Closer.png)
This image displays the performance report after successfully closing **100 trades**. The report provides a comprehensive summary of the operation, including the total realized P/L, price movement during execution, and total time.

* **Execution Speed Analysis:**
    * **Total Time:** 100 trades were closed in **40.44 seconds**.
    * **Performance Rate:** An execution rate of up to **2.47 trades per second** (or ~148 trades per minute).

### 4. The Cleaner Script (MT4_Execution_Suite_Cleaner.mq4)
A simple utility to remove visual clutter from the chart, providing a clean slate for analysis.

**Before running the script:** The chart is cluttered with graphical objects (arrows, dots) left behind by indicators, making analysis difficult.
![Chart Before Cleaner](Documentation/Before_MT4_Execution_Suite_Cleaner.png)

**After running the script:** With a single click, the script removes all unwanted objects, leaving a clean chart ready for clear analysis.
![Chart After Cleaner](Documentation/After_MT4_Execution_Suite_Cleaner.png)

---
## Key Features of the Suite

* **Superhuman Execution Speed:** Execute trades at a velocity impossible for a human, with rates exceeding **3 trades per second**, giving you a decisive edge in fast-moving markets.
* **Universal Compatibility:** By using **Points** as the standard unit for SL/TP in the Opener, the tools work with flawless precision across all instruments (Forex, Gold, Indices, etc.).
* **Intelligent Reporting:** Get detailed performance reports after every operation, with clear reasons for any emergency stops, ensuring full transparency.
* **Complete Trading Workflow:** The suite provides a full lifecycle for trade management, from opening and monitoring to closing and workspace cleanup.

---
## Installation
1.  Download the project repository.
2.  Open your MetaTrader 4 terminal.
3.  Go to `File` > `Open Data Folder`.
4.  Copy the `MQL4` folder from this project and paste it into your MT4 Data Folder. When prompted, agree to merge the folders.
5.  In your MT4 terminal, go to the "Navigator" window, right-click on "Scripts" and select "Refresh", or simply restart the terminal.

---
## License
This project is licensed under the MIT License. See the `LICENSE` file for details.
