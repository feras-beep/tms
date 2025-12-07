# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **nTMS-based GBM Survival Prediction Calculator** - a single-page web application that implements a logistic regression model for predicting 12-month survival probability in Glioblastoma patients. The model incorporates navigated Transcranial Magnetic Stimulation (nTMS) cortical excitability metrics alongside traditional clinical factors.

## Architecture

The entire application is contained in a single `index.html` file with:
- **Embedded CSS** (lines 7-293): Responsive styling with CSS Grid layout, gradient backgrounds, and mobile breakpoints
- **HTML structure** (lines 295-441): Two-panel layout (input form + results display)
- **Embedded JavaScript** (lines 443-606): Logistic regression calculation engine with real-time input updates

## Key Components

### Logistic Regression Model (lines 446-456)
The `modelCoefficients` object contains the validated coefficients from a King's College Hospital GBM cohort study (n=77 patients). Key predictors:
- **CES (Cortical Excitability Score)**: 0-2 scale, higher = worse survival
- **IMES (IntraM1 Excitability Score)**: Ratio metric, higher = better survival
- Clinical factors: age, MGMT methylation, extent of resection, tumor volume, location

### Core Functions
- `calculatePrediction()`: Main entry point, orchestrates calculation and display
- `computeLogisticRegression(inputs)`: Applies logistic function to compute survival probability
- `generateInterpretation(inputs, prediction)`: Creates clinical interpretation of risk factors

## Development

No build system or dependencies - open `index.html` directly in a browser to run. The application auto-calculates on input changes with 300-500ms debouncing.

## Static Assets

- `ntms-image.png`: Header visualization of nTMS brain mapping
- `TMS GBM Prognostication for CALCULATOR (1).xlsx`: Source data spreadsheet (not used by the web app)
