---
title: Weather Forecast Display
description: How to display weather forecasts in Bharat Signage using real-time data from online sources.
sidebar_position: 3
---

_Bharat Signage_ allows you to display **weather forecasts** on screen using real-time data from the internet. The forecast includes an **icon**, **date**, and **temperature range** for each day. You may also include a custom text heading above the forecast.

## How to Set Up Weather Display

1. Create a new content item with the type **“Weather”**.
2. Add it to your playlist.
3. (Optional) Use the predefined layout **“With side panels”** as a template for easier setup.

You can display the forecast for **up to 4 days**:

- **Vertically**: Set columns to `1`
- **Horizontally**: Set columns to `4`

### Temperature Units

By default, temperatures are shown in **°C (Celsius)**. To switch to **°F (Fahrenheit)**:

- Enable the option **“Temperature in °F”**
- Change the **Text template** to:  
  `EEEE': %.0f to %.0f °F'`

### Icon Style

You can customize the **style of weather icons** by choosing from available icon sets in the **Edit Content** page.

## Weather Data Sources

Bharat Signage supports multiple online weather APIs. Most of them offer a **free plan**, though some require **registration and API keys**.

Set up the weather source in the web interface via:  
**Settings → Device Settings**

| Weather Provider       | Registration Required | Free Tier Limits       | API Key Setup                                                       | Device Settings Value                                              |
| ---------------------- | --------------------- | ---------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------ |
| **Open-Meteo**         | ❌ No                 | 10,000 requests/day    | No API key needed                                                   | `Weather source: Open-Meteo`                                       |
| **OpenWeatherMap**     | ✅ Yes                | 60 requests/min        | [Get API Key](https://home.openweathermap.org/api_keys)             | `Weather source: OpenWeatherMap (hourly) API key: {your_api_key}`  |
| **HERE Maps**          | ✅ Yes                | 250,000 requests/month | [Sign up](https://developer.here.com/sign-up?create=Freemium-Basic) | `Weather source: HERE Destination weather API key: {your_api_key}` |
| **MET Norway (yr.no)** | ❌ No                 | Fair usage             | No API key needed                                                   | `Weather source: MET Norway (yr.no)`                               |

> ⚠️ **Note:** Weather forecasts are **cached for 1 hour** per location. A single free account is typically sufficient for multiple devices. For **50+ devices** or **guaranteed uptime**, consider switching to a paid plan.
> 📜 Be sure to review the **license terms** of your selected weather provider. Some services require attribution or prohibit commercial use.

## Troubleshooting Weather Updates

Each time Bharat Signage fetches weather data, a log entry is created. You can view it in:  
**Information → Log**

Example of a successful update:
2020-10-25 17:47:20 INFO WeatherReader - Weather refreshed (location=Punta Arenas)

Example of a missing API key:
:::danger[Error]

2020-10-25 21:46:16 WARN WeatherReader - Can't refresh weather: OpenWeatherMap API key not found, please obtain it on [OpenWeatherMap](https://home.openweathermap.org/users/sign_up) and enter it in the Device settings

:::
This feature enables your digital signage screens to provide timely weather updates alongside your regular content, improving viewer engagement and utility.
