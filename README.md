# ESP32 + DHT22 Live Dashboard

A single-page HTML dashboard that displays live temperature and humidity readings from an ESP32 + DHT22 sensor, with auto-refresh and a historical chart.

## Overview

This is a static, framework-free frontend that polls a backend API for sensor data and renders it as:
- Live current temperature and humidity values
- Min/max stats over the recent history window
- A line chart (Chart.js) showing the last 60 readings over time
- A connection status badge (Live / Server unreachable)

It is designed to be deployed as a single static HTML file (e.g. via GitHub Pages, Render Static Site, or any static host) and consumes data from the `esp32-backend` API.

## Tech Stack

- Plain HTML, CSS, and vanilla JavaScript — no build step required
- **Chart.js 4.4.1** (loaded via CDN) for the history line chart
- Fetches data from the deployed backend over HTTPS

## File Structure# esp32-dashboard
