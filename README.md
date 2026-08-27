# Walmart Sales Dashboard

An interactive **Walmart Sales Dashboard** built using **HTML, CSS, JavaScript, Chart.js, and Papa Parse**. The dashboard loads Walmart sales data from a CSV file and provides interactive filters and visualizations for analyzing sales performance.

## 🚀 Live Demo

[Walmart Sales Dashboard](https://velvety-peony-651b66.netlify.app/?utm_source=chatgpt.com)

## 📊 Dashboard Features

* **Total Sales** – Displays total sales based on the selected filters.
* **Average Weekly Sales** – Shows the average weekly sales.
* **Best Store** – Identifies the store with the highest sales.
* **Record Count** – Displays the number of records currently being analyzed.
* **Weekly Sales Trend** – Line chart showing sales over time.
* **Sales by Store** – Bar chart showing the top-performing stores.
* **Holiday vs Non-Holiday Sales** – Pie chart comparing sales during holidays and non-holidays.
* **Store Filter** – Filter the dashboard by individual store.
* **Year Filter** – Filter the dashboard by year.
* **Reset Filters** – Quickly return to the complete dataset.

## 🛠️ Technologies Used

* **HTML5** – Dashboard structure
* **CSS3** – Styling and responsive layout
* **JavaScript** – Data processing and interactivity
* **Chart.js** – Data visualization
* **Papa Parse** – Reading and processing the CSV file
* **Netlify** – Deployment
* **GitHub** – Version control and source code hosting

## 📁 Project Structure

```text
walmart_analysis/
│
├── index.html
├── index.css
├── Walmart_Sales.csv
├── README.md
└── .gitattributes
```

## 📂 Dataset

The dashboard uses the `Walmart_Sales.csv` dataset.

The dataset contains the following fields:

| Column         | Description                              |
| -------------- | ---------------------------------------- |
| `Store`        | Store identification number              |
| `Date`         | Weekly sales date                        |
| `Weekly_Sales` | Sales for the given store and week       |
| `Holiday_Flag` | Indicates whether the week was a holiday |
| `Temperature`  | Temperature during the week              |
| `Fuel_Price`   | Fuel price during the week               |
| `CPI`          | Consumer Price Index                     |
| `Unemployment` | Unemployment rate                        |

## 🔄 How It Works

The dashboard loads the CSV file using **Papa Parse**:

```javascript
Papa.parse("Walmart_Sales.csv", {
    download: true,
    header: true,
    skipEmptyLines: true
});
```

The data is then filtered according to the selected **Store** and **Year**.

Whenever a filter changes, the dashboard recalculates the metrics and redraws the charts using the filtered data.

## 📈 Visualizations

### Weekly Sales Trend

A line chart is used to visualize how Walmart's weekly sales change over time.

### Sales by Store

A bar chart compares total sales across stores and highlights the top-performing stores.

### Holiday vs Non-Holiday Sales

A pie chart compares the proportion of sales generated during holiday and non-holiday weeks.

## 🎛️ Interactive Filters

The dashboard includes two main filters:

**Store**

```text
All Stores
Store 1
Store 2
Store 3
...
```

**Year**

```text
All Years
2010
2011
2012
```

Changing either filter updates the dashboard metrics and charts.

## 💻 Running the Project Locally

1. Clone the repository:

```bash
git clone https://github.com/ParthGitthub/walmart_analysis.git
```

2. Open the project in VS Code.

3. Make sure these files are in the same folder:

```text
index.html
index.css
Walmart_Sales.csv
```

4. Run the project using **Live Server**.

5. Open the local URL provided by Live Server.

> Using Live Server is recommended because the dashboard loads the CSV file through JavaScript.

## 🌐 Deployment

The project is deployed using **Netlify** and connected to the GitHub repository.

Any new changes pushed to the connected GitHub branch can trigger a new deployment.

## 🎯 Project Objective

The objective of this project is to demonstrate how raw sales data can be transformed into an interactive dashboard that makes it easier to:

* Analyze sales trends
* Compare store performance
* Understand holiday sales patterns
* Filter data dynamically
* Present business data visually
* Build a practical data analytics portfolio project

## 📌 Future Improvements

Possible improvements for future versions include:

* Add monthly and yearly sales analysis
* Add sales vs temperature analysis
* Add sales vs fuel price analysis
* Add CPI and unemployment analysis
* Add more advanced KPI cards
* Add date-range filtering
* Add downloadable reports
* Add additional dashboard visualizations
* Improve mobile responsiveness

## 👨‍💻 Author

**Parth**

GitHub: [ParthGitthub](https://github.com/ParthGitthub)

---

⭐ If you found this project useful, consider giving the repository a star.
