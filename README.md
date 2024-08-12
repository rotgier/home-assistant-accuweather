# home-assistant-accuweather
Custom Accuweather integration for Home Assistant.

It is the same code as in the official Accuweather integration: https://github.com/home-assistant/core/tree/dev/homeassistant/components/accuweather 

Only the support for hourly weather forecast that requires a separate API key was added.

Since the free Accuweather API is limited to 50 requests per day and the official HA Accuweather integration already uses 36 requests (1 each 40 minutes) for current weather conditions and another 4 requests (1 each 6 hours) for daily forecast updates, this integration allows user to provide additional api key for hourly forecast updates (1 each 40 minutes)

The additional API key for hourly weather forecast can be obtained in the same exact way as the main API key. The setup is described here: https://www.home-assistant.io/integrations/accuweather/ . Simply to get the additional API key, create a second account at https://developer.accuweather.com/ and there a second application.

Note: the hourly weather forecast is limited to 12 hours by the Accuweather API.
