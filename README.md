# Solar Energy Production Analysis

This Excel workbook contains various analyses and calculations on a dataset of solar energy production. The dataset includes information such as the name, id, address, date, kWh production, public URL, installation date, and uid of each solar installation. The workbook performs several data processing tasks and analyses, including setting data validation rules, creating charts, identifying max/min values, calculating days since installation, using VLOOKUP, and generating a summary report.

## Table of Contents

- [Dataset](#dataset)
- [Data Validation](#data-validation)
- [Charts](#charts)
- [Max/Min Values](#maxmin-values)
- [Days Since Installation](#days-since-installation)
- [VLOOKUP](#vlookup)
- [Cumulative kWh Production](#cumulative-kwh-production)
- [Summary Report](#summary-report)
- [Usage](#usage)
- [License](#license)

## Dataset

The dataset used in this workbook includes the following columns:

- `name`: Name of the site
- `id`: Unique identifier for the site
- `address`: Address of the site
- `date`: Date of kWh production entry
- `kWh`: Energy production in kilowatt-hours
- `public_url`: Public URL of the site
- `installationDate`: Date when the installation was completed
- `uid`: Unique user identifier

## Data Validation

A data validation rule was set up for the `kWh` column to ensure that only positive numbers can be entered. This helps maintain data integrity by preventing invalid entries.

## Charts

A line chart was created to show the trend of kWh production over time. Additionally, a trendline was added to the chart to visualize the general production trend.

## Max/Min Values

The maximum and minimum energy production values in the `kWh` column were identified using the `MAX` and `MIN` functions.

## Days Since Installation

The workbook calculates the number of days since each installation by finding the difference between the `installationDate` and today's date using the `TODAY()` function.

## VLOOKUP

The `VLOOKUP` function is used to find the address of a specific `id`. This allows quick lookup of site details based on the unique identifier.

## Cumulative kWh Production

The cumulative kWh production for each `id` over time was calculated using the `SUMIF` function. This provides a running total of energy production for each site.

## Summary Report

A summary report was created to show the total production, total revenue, and average revenue per entry. This provides a high-level overview of the dataset's performance metrics.

### Total Production

Calculated using the `SUM` function to sum up all kWh values.

### Total Revenue

Calculated using the `SUM` function to sum up all revenue values (assuming a `Revenue` column is present).

### Average Revenue per Entry

Calculated using the `AVERAGE` function to find the mean revenue per entry.

## Usage

1. Open the Excel workbook.
2. Review the dataset and make sure it is properly formatted.
3. Check the `kWh` column for data validation rules ensuring positive values.
4. View the line chart showing kWh production trends over time.
5. Identify the maximum and minimum kWh production values.
6. Check the number of days since each installation.
7. Use the `VLOOKUP` function to find the address of specific `id`s.
8. Review the cumulative kWh production for each site.
9. Analyze the summary report for total production, total revenue, and average revenue per entry.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
