# Uber Supply and Demand Case Study

This repository contains a Jupyter Notebook that analyzes Uber's supply and demand data over a two-week period. The analysis aims to provide insights into various aspects of Uber's operations, including trip completion, driver availability, and demand patterns.

## Table of Contents

1. [Introduction](#introduction)
2. [Data Overview](#data-overview)
3. [Key Insights](#key-insights)
4. [Usage](#usage)
5. [Dependencies](#dependencies)
6. [Contributing](#contributing)
7. [License](#license)

## Introduction

This case study focuses on understanding Uber's supply and demand dynamics by analyzing data collected over two weeks. The analysis answers several key questions related to trip completion, driver availability, and demand patterns. The insights derived from this analysis can help in optimizing driver schedules, improving service availability, and enhancing overall operational efficiency.

## Data Overview

The dataset used in this analysis contains the following columns:

- **Date**: The date of the record.
- **Time (Local)**: The hour of the day (in 24-hour format).
- **Eyeballs**: The number of users who opened the Uber app.
- **Zeroes**: The number of users who did not find a ride.
- **Completed Trips**: The number of completed trips.
- **Requests**: The number of ride requests.
- **Unique Drivers**: The number of unique drivers available.

The dataset is loaded into a Pandas DataFrame for analysis.

## Key Insights

The analysis answers the following questions:

1. **Which date had the most completed trips during the two weeks?**
   - The date with the most completed trips was **22-Sep-12** with a total of **248** trips.

2. **What was the highest number of completed trips within a 24-hour period?**
   - The highest number of completed trips within a 24-hour period was **248**.

3. **Which hour of the day had the most requests during the two-week period?**
   - The hour with the most requests was **23:00**.

4. **What percentage of all zeroes during the two-week period occurred on weekends (Friday at 5 pm to Sunday at 3 am)?**
   - **44.86%** of all zeroes occurred on weekends.

5. **What is the weighted average ratio of completed trips per driver during the two-week period?**
   - The weighted average ratio of completed trips per driver was **0.51**.

6. **In drafting a driver schedule in terms of 8-hour shifts, when are the busiest 8 consecutive hours over the two-week period in terms of unique requests?**
   - The busiest 8-hour period is from **22:00 to 06:00**.

7. **True or False: Driver supply always increases when demand increases during the two-week period.**
   - **False**. The demand for Uber requests does not guarantee an increase in the supply of drivers.

8. **In which 72-hour period is the ratio of Zeroes to Eyeballs the highest?**
   - The 72-hour period with the highest zeroes-to-eyeballs ratio starts at **2012-09-18 04:00:00** with a ratio of **0.37**.

9. **If you could add 5 drivers to any single hour of every day during the two-week period, which hour should you add them to?**
   - Add 5 drivers to **23:00** to address the largest absolute shortage.

10. **True or False: There is exactly two weeks of data in this analysis.**
    - **False**. The data does not cover exactly two weeks.

11. **Looking at the data from all two weeks, which time might make the most sense to consider a true "end day" instead of midnight?**
    - The true "end day" can be considered at **4:00** when both supply and demand are at their natural minimums.

## Usage

To run the analysis:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/uber-supply-demand-analysis.git
   ```

2. Navigate to the project directory:
   ```bash
   cd uber-supply-demand-analysis
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Uber_Case_Study.ipynb
   ```

5. Run the cells in the notebook to perform the analysis.

## Dependencies

The analysis requires the following Python libraries:

- **NumPy**
- **Pandas**
- **Matplotlib**
- **Seaborn**

You can install these dependencies using the provided `requirements.txt` file.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
