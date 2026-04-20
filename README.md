# Statistical Simulator: Outlier Impact (Weibull)

An interactive Single Page Application (SPA) to visualize in real-time how early failures (outliers) influence and distort the Probability Density Function (PDF) in parametric statistical models.

## How to use it

1. **Live Demo:** Open the link provided by GitHub Pages to launch the tool directly in your browser.
2. **Data Customization:** Upload or modify the `data.csv` file located in the root of the repository. Enter your values (e.g., operational hours, cycles, age at failure) by writing one number per line. The system automatically ignores text, headers, and null values.
3. **Interactive Analysis:** Use the on-page controls to exclude or include historical data (e.g., infant mortality events) and observe the instantaneous impact on the curve's parameters.

## Technical Info

* **No Backend:** The application runs entirely client-side using JavaScript. It requires no Python, server, or database.
* **Parametric Calculation:** It utilizes Linear Regression on Median Ranks (Bernard's Approximation) to dynamically estimate the Shape (&beta;) and Scale (&eta;) parameters.
* **External Libraries:** Chart.js (via CDN) for rendering the distribution chart.
