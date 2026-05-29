# Weather Data Pipeline

## API Used

Open-Meteo API

Reason:

* Free to use
* No API key required
* Easy structured JSON response

## Pipeline Steps

1. Fetch weather data from Open-Meteo API
2. Transform JSON response into tabular format
3. Add derived field:

   * temperature_category
4. Store transformed data in BigQuery

## Error Handling

* API request exceptions handled
* Missing data validation added
* Logging included

## SQL Summary Query

The SQL query calculates average temperature by category.

## Production Improvements

### Scheduling

Use cron jobs or Apache Airflow.

### Failure Monitoring

Use logging and email alerts.

### Scaling

Use partitioned BigQuery tables and batch processing.
