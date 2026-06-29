# Postman API Testing Project (Open-Meteo)

## Overview
This project tests the Open-Meteo Weather Forecast API using Postman.
It validates API responses such as status codes and forecast data structure.

## API Used
https://open-meteo.com/en/docs

## Test coverage:
- Happy path: smoke test, required fields, data types, data consistency
- Boundary tests: latitude/longitude edge values (+/-179, +/-180)
- Negative tests: invalid latitude and timezone inputs with error validation

## The tests validate:
- API response status codes
- Response schema consistency
- Geographic boundary behavior
- Input validation handling
- Forecast data integrity

## Tools
- Postman
- Newman (optional for CLI execution)

## How to run (optional automation mode):

Install Newman:
npm install -g newman

Run collection:
newman run Weather_Forecast_API.postman_collection.json -e Sydney-Australia.postman_environment.json
