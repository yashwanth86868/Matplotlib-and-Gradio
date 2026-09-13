# 📊 Matplotlib & Gradio — Sales and Profit Visualization

A beginner-friendly Python project that uses **Pandas**, **Matplotlib**, and **Gradio** to analyze monthly sales and profit data and display different visualizations through an interactive web interface.

## 🚀 Project Overview

This project explores a small sales and profit dataset containing information for six months:

- January
- February
- March
- April
- May
- June

The project first creates different charts using Matplotlib. Then, it uses Gradio to build an interactive application where the user can select a chart type and view the corresponding visualization.

## 🛠️ Technologies Used

- **Python** — Programming language
- **Pandas** — Creating and handling the dataset
- **NumPy** — Numerical computing
- **Matplotlib** — Creating charts and visualizations
- **Gradio** — Building an interactive web interface
- **Jupyter Notebook** — Developing and running the project

## 📁 Dataset

The project uses a manually created dataset with three columns:

| Month |   Sale | Profit |
| ----- | -----: | -----: |
| Jan   | 10,000 |  2,000 |
| Feb   | 12,000 |  3,000 |
| March | 15,000 |  4,000 |
| April | 13,000 |  2,500 |
| May   | 15,500 |  3,500 |
| June  | 17,000 |  5,000 |

The dataset is stored in a Pandas DataFrame.

## 📈 Matplotlib Visualizations

The notebook includes the following charts:

### 1. Line Plot

Shows the monthly sales trend and helps understand how sales change over time.

### 2. Stacked Bar Chart

Displays sales and profit together for each month using stacked bars.

### 3. Pie Chart

Shows the contribution of each month's profit to the total profit.

### 4. Scatter Plot

Displays the relationship between sales and profit.

### 5. Histogram

Shows the distribution of sales values.

### 6. Box Plot

Provides a visual summary of the profit values and helps identify the spread of the data.

## 🌐 Gradio Application

The project includes an interactive Gradio application named:

> **Sales & Profit Visual Insight**

The user can select one of the following visualization types:

- Line Plot
- Pie Chart
- Scatter Plot
- Histogram
- Stacked Bar Chart
- Box Plot

After selecting a chart type, Gradio calls the `generate_plot()` function and displays the selected Matplotlib visualization.

## 🔄 How the Application Works

```text
Sales and Profit Data
          ↓
     Pandas DataFrame
          ↓
   Matplotlib Plotting
          ↓
   generate_plot() Function
          ↓
     Gradio Interface
          ↓
 Select Chart and View Output
```

## ⚙️ Installation

Install the required libraries using pip:

```bash
pip install numpy pandas matplotlib gradio jupyter
```

Or create a `requirements.txt` file with:

```text
numpy
pandas
matplotlib
gradio
jupyter
```

Then install the dependencies:

```bash
pip install -r requirements.txt
```

## ▶️ How to Run the Project

### Option 1: Run using Jupyter Notebook

1. Clone this repository.
2. Open the notebook `Matplotlib full.ipynb`.
3. Install the required libraries.
4. Run the notebook cells in order.
5. Execute the Gradio cell to launch the interactive application.

### Option 2: Run using Google Colab

1. Upload the notebook to Google Colab.
2. Run the installation cell.
3. Execute the Matplotlib examples.
4. Run the Gradio application cell.
5. Open the Gradio interface link displayed by the notebook.

## 💻 Main Function

The Gradio application uses a function named `generate_plot()`.

This function:

1. Receives the selected chart type.
2. Creates a Matplotlib figure.
3. Checks which visualization the user selected.
4. Generates the corresponding chart.
5. Returns the figure to Gradio.

Example structure:

```python
def generate_plot(plot_type):
    fig = plt.figure(figsize=(10, 5))

    if plot_type == "Line Plot":
        # Create a line plot

        pass

    elif plot_type == "Histogram":
        # Create a histogram

        pass

    return fig
```

## 🎯 Learning Objectives

Through this project, I learned how to:

- Create a DataFrame using Pandas.
- Work with sales and profit data.
- Create different types of Matplotlib charts.
- Add titles, labels, legends, and grids to plots.
- Understand when to use different visualization types.
- Create a reusable plotting function.
- Build an interactive interface using Gradio.
- Connect Matplotlib figures to a Gradio application.

## 📌 Project Highlights

- Six different visualization types
- Beginner-friendly sales and profit dataset
- Reusable `generate_plot()` function
- Interactive chart selection using Gradio
- Visual analysis of sales and profit data

## 🔮 Future Improvements

- Add more months and real-world sales data.
- Allow users to upload their own CSV files.
- Add filters for months and financial metrics.
- Display total sales and total profit.
- Add interactive dashboards.
- Improve the visual design of the Gradio interface.
- Deploy the application online.

## 👨‍💻 Author

**Yashwanth Balija**

Learning Python, data visualization, and machine learning tools through practical projects.

## ⭐ Support

If you find this project useful, consider giving the repository a star ⭐.

Happy Learning! 🚀
