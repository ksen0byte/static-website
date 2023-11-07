# GA4 USD/UAH Exchange Rate Monitor

This project sets up a static website hosted on GitHub Pages and integrates Google Analytics 4 (GA4) to monitor user metrics. It includes a backend worker implemented as a GitHub Actions workflow, which fetches the current USD/UAH exchange rate from the National Bank of Ukraine's API and pushes this data as an event to GA4.

## Overview

The purpose of this project is to track the exchange rate between the Ukrainian hryvnia (UAH) and the US dollar (USD) using a custom event in GA4. This event is triggered daily via a GitHub Actions workflow, ensuring that the exchange rate data is consistently updated in the analytics dashboard.

## Workflow

The `.github/workflows/daily-rate-update.yml` file contains the workflow definition that automates the fetching of the current exchange rate and its submission to GA4.

## Usage

To view the exchange rate data:
1. Visit the [static website](https://ksen0byte.github.io/static-website/).
2. Navigate to the [GA4](https://analytics.google.com/analytics/web/#/p414437146/reports/intelligenthome) property to monitor the `update_rate` event under the Reports section.
