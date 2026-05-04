# AI-Based-UK-Flood-Assessment
An AI-powered dashboard that provides hyper-local flood risk assessments for any UK postcode. This tool integrates historical Environment Agency data, live flood alerts, and real-time rainfall forecasts into a single, professional PDF report (https://www.kaggle.com/code/minervasdatalab/flood-gemma1gradio1)

## Key Features
Historical Risk Lookup: Queries a local Environment Agency dataset for long-term probability bands and insurance suitability.  

Live EA Alerts: Fetches real-time warnings from the Environment Agency API within a 15km radius of the target location.  

48-Hour Rainfall Forecast: Utilizes the Open-Meteo API to predict precipitation levels and evaluate flash flood relevance.  

AI-Powered Summaries: Uses Gemma 2B (quantized via BitsAndBytes) to interpret data and provide grounded safety summaries.  

Professional PDF Export: Generates an A4 report using WeasyPrint for easy sharing and record-keeping.  

## Tech Stack
Model: Google Gemma 2B-it (4-bit quantization).  

Framework: Gradio for the web interface.  

APIs: Environment Agency (Flood Monitoring), Open-Meteo, Postcodes.io.  

Libraries: transformers, bitsandbytes, weasyprint, pandas.  

