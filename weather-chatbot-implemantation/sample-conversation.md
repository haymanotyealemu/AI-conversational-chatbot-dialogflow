## Successful Scenario 1 – Valid Coordinates

User: Weather at 33.7490 -84.3880  
Bot: The current weather at latitude 33.7490 and longitude -84.3880 is sunny with a temperature of 75°F.

Intent Matched: Weather_By_Coordinates  
Parameters Extracted:
- latitude: 33.7490
- longitude: -84.3880
Fulfillment: Webhook response (Inline Editor)
## Scenario 2 – Missing Longitude

User: Weather at 33.7490  
Bot: Please provide the longitude value as well.

Intent Matched: Weather_By_Coordinates  
Missing Parameter: longitude  
System Prompt Triggered: Yes
## Scenario 3 – Invalid Coordinates

User: Weather at 200 500  
Bot: The provided coordinates are outside the valid geographic range. Please enter valid latitude (-90 to 90) and longitude (-180 to 180).
## Scenario 4 – Alternative Phrase

User: Can you get the forecast for 40.7128 -74.0060?  
Bot: The current weather at latitude 40.7128 and longitude -74.0060 is cloudy with 68°F.

Intent Matched: Weather_By_Coordinates  
