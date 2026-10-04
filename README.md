# 🙡 TJ Souabny 🙢

Math & CS at the University of Pennsylvania

Interested in topology, statistics, and using math to understand investing.

## Currently building

### [TDA for Financial Data](https://github.com/tariksouabny/tda_distance)
<img width="400" height="300" alt="image" src="https://github.com/user-attachments/assets/b8135e6f-db99-4414-8013-97a0dfcdc91c" />
<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/df8eb43d-88da-43fc-9963-ab39a962cfca" />

I’m developing a Python library for applying topological data analysis to financial datasets.

The project started as an S&P 500 research pipeline: collect stock returns, convert their correlations into distances, and examine the resulting structure using persistent homology and Mapper. The current implementation computes connected components and loops with Ripser and generates persistence diagrams and interactive market maps.

I’ve added configurable analysis windows, data caching, a command-line interface, and tests. My next step is adding functionality, the final deliverable will be a reusable library for answering research questions with financial data

## Completed research projects

### [Zero-GC FIX Parser](https://github.com/tariksouabny/zerogc_fixparser)

Parsing financial messages while reusing memory using Java.

I implemented byte-level tag parsing and checksum validation using a preallocated buffer. Field values are stored as offsets/lengths instead of being converted into strings during the fact.

The repo includes JUnit tests and a JMH benchmark. Average performance was **19.5 million parses per second** for a fixed test message, or 51 nanoseconds / parse. 

See: [Mechanical Sympathy, Martin Thompson](https://mechanical-sympathy.blogspot.com/2013/07/java-garbage-collection-distilled.html)

### [RSI Mean-Reversion Backtester](https://github.com/tariksouabny/quant-rsi-backtester)

A Python research project examining RSI-based trading rules across S&P 500 equities.

In my notebook, I used RSI signals, moving-average filters, and position sizing is scaled by ATR. I compared the strategy with S&P returns and an equal-weight benchmark. I separated earlier and later periods for the evaluation phase. The saved run underperformed both benchmarks on return & Sharpe ratio, but experienced a smaller maximum drawdown.

## Tools

**Python · Java · NumPy · pandas · scikit-learn · Ripser · KeplerMapper · JMH · JUnit**
