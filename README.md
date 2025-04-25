## Subscription Level Analysis
This project analyzes factors influencing subscription levels in a real estate dataset containing property listings across different cities. The goal is to uncover patterns, relationships, and variable importance impacting subscription behaviors.

## Project Overview
Dataset Size: 3500 entries and 8 columns.

Post-cleaning: 3489 unique rows (after duplicate removal).

Balance: Subscriptions are evenly spread across different levels, indicating a balanced dataset.

### Data Cleaning Highlights
Missing Values:

subscription_level: 3 missing values.

has_online_tour: 2810 missing values.

Key Observations:

has_online_tour data is unavailable for low vacancy_level entries.

Dataset entries are available only up to June 2019.

Feature Engineering:

Extracted year, month, and day from date_of_subscription to analyze time-based effects on subscription levels.

### Key Findings
#### Day and Month Effects:

More subscriptions happen on Fridays and Sundays.

Subscription activity spikes at the start and end of each month.

Higher subscription levels occur during the last quarter of the year — possibly influenced by the holiday season.

#### City Insights:

City ID 152 has the highest number of subscriptions.

Generally, high lead volume results in more subscriptions, but:

High photo quality can compensate for low lead volume, still leading to high subscriptions in certain cities.

#### Feature Dependencies:

Clear dependency observed between:

vacancy_level and photo_quality.

vacancy_level and lead_volume.

#### Variable Importance:

Top influential features impacting subscription level:

city_id

day (of the week)

month
