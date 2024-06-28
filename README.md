# DavisLoop-Live-Weather-Monitoring-Dashboard
 Realtime Graph for Davis Loop Data using MQTT

This project displays real-time weather data from a Davis personal weather station using MQTT and Chart.js. It provides a live graph of various weather metrics and displays current weather statistics and forecasts.

## Project Screenshot

<img src="https://www.digitalurban.org/wp-content/uploads/2024/06/Screenshot-2024-06-27-at-15.48.35-1024x631.png" alt="Live Weather Graph Interface" width="500"/>

*Screenshot of the Live Weather Graph interface*

## Live Demo

Check out the live demo of the weather graph here: [Live Weather Graph Demo] (https://www.finchamweather.co.uk/weathergraph.htm)

## Features

- Real-time weather data visualization
- MQTT connection for live updates
- Responsive design
- Display of key weather statistics:
  - Max Wind Speed
  - Max and Min Temperature
  - Max and Min Pressure
- Weather forecast display
- Mobile-friendly interface

## Technologies Used

- HTML5
- CSS3
- JavaScript
- [Paho MQTT JavaScript Client](https://eclipse.org/paho/clients/js/)
- [Chart.js](https://www.chartjs.org/)
- [Date-fns Chart.js Adapter](https://github.com/chartjs/chartjs-adapter-date-fns)

## Setup

1. Clone this repository
2. Open `index.html` in a web browser

## MQTT Configuration

The application connects to the MQTT broker at `mqtt.cetools.org`. It subscribes to two topics:

- `personal/ucfnaps/downhamweather/loop`: For real-time weather data
- `personal/ucfnaps/eink/met`: For weather forecasts

- 'edit these for your own Davis Loop Mqtt feed and forecast, the forecast can be excluded as needs be.

## Weather Metrics Displayed

- Wind Speed (mph)
- Temperature (°C)
- Solar Radiation (W/m²)
- Rain Amount (mm)
- Pressure (mbar)

## Chart Features

- Time-based x-axis
- Multiple y-axes for different metrics
- Automatic data point limitation for performance
- Responsive design

## Customization

You can customize the chart appearance, data retention period, and update intervals by modifying the JavaScript code in the `<script>` section.

## Contributing

Contributions, issues, and feature requests are welcome. Feel free to check [issues page](https://github.com/yourusername/live-weather-graph/issues) if you want to contribute.

## License

[MIT](https://choosealicense.com/licenses/mit/)