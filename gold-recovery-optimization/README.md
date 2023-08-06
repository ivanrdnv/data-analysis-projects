# Machine Learning Model Prototype for "Numbers" Company
## Overview

This project aims to develop a machine learning model prototype for "Numbers," a company that specializes in providing solutions for the efficient operation of industrial enterprises. The model's primary objective is to predict the gold recovery coefficient from gold-bearing ore.

## Problem Statement

The main challenge is to predict the gold recovery coefficient accurately. By forecasting this coefficient, "Numbers" can identify optimal operating conditions for its industrial clients, thus minimizing losses and enhancing overall productivity.


## Dataset Description
The data is distributed among three files:

    gold_industry_train.csv: Training dataset
    gold_industry_test.csv: Test dataset
    gold_industry_full.csv: Original dataset

**Technological Process**

    Rougher feed: Original raw material
    Rougher additions (or reagent additions): Flotation reagents - Xanthate, Sulphate, Depressant
        Xanthate: Xanthogenate (promoter or flotation activator)
        Sulfate: Sodium sulfate (sulfide sodium in this production)
        Depressant: Sodium silicate
    Rougher process: Flotation
    Rougher tails: Tailings after flotation
    Float banks: Flotation cells
    Cleaner process: Cleaning
    Rougher Au: Rougher gold concentrate
    Final Au: Final gold concentrate

**Stage Parameters**

    air amount: Air volume
    fluid levels: Liquid level
    feed size: Raw material granule size
    feed rate: Feeding rate

**Feature Naming Convention**

[stage].[parameter_type].[parameter_name]

Possible values for the [stage] block:

    rougher: Flotation
    primary_cleaner: Primary cleaning
    secondary_cleaner: Secondary cleaning
    final: Final characteristics

Possible values for the [parameter_type] block:

    input: Raw material parameters
    output: Product parameters
    state: Parameters characterizing the current stage state
    calculation: Calculated characteristics

## Formula for Enrichment Efficiency
$$Recovery = \frac{C\cdot(F-T)}{F\cdot(C-T)}\cdot100\% $$

Where:
- C is the concentration of gold in the final concentrate.
- F is the mass flow rate of gold in the feed.
- T is the mass flow rate of gold in the tailings.

# Conclusion 
The successful development of the machine learning model prototype will empower the company to predict the gold recovery coefficient accurately.
