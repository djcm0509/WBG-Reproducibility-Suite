WBG Reproducibility & Automated Testing Suite

This repository contains an automated framework designed for World Bank Reproducible Research reviews. It ensures data integrity through statistical validation and containerized environments.

Features

Statistical Verifier: CLI tool to perform 2-sample Z-tests and summary statistic comparisons.

Metadata Validator: Ensures JSON metadata aligns with WBG documentation standards.

Dockerized Environment: Zero-config setup for peer reviewers.

CI/CD Integration: Automated reproducibility checks via GitHub Actions.

Quick Start

Using Docker

Build the image: docker build -t wbg-verifier .

Run the suite: docker run -it wbg-verifier

Manual Setup

Install dependencies: pip install -r requirements.txt

Run data check: python wbg_verifier.py --raw data.csv --target output.csv --col "gdp_growth"
