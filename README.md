# :hospital: dExtension :computer:

Keeping track of blood sugar levels can often feel overwhelming, especially on top of a busy workweek.

That's why I sought to build dExtension, a tool that enables developers with diabetes to easily see their blood sugar data within their VS Code programming environment, in real-time - all without disrupting their workflow.

![dExtension full screen app view](/assets/full_screen.png)

## Features

In the dExtension status bar item, users are able to see their latest blood glucose reading, their glucose trend arrow (rate of change in glucose levels over the last minute), the difference in glucose levels between their last two readings, and the amount of minutes that have elapsed since their last reading time.

### :arrow_upper_right: Status Bar Item:

![dExtension status bar item](/assets/status_bar.png)

In addition to live blood sugar readings, users of dExtension are also able to view a historical three-hour trend graph that will automatically match their VS Code theme preference (light / dark).

### :chart_with_upwards_trend: Trend Graph (Light Color Theme):

![trend graph, light color theme](/assets/trend_graph_light.png)

### :chart_with_downwards_trend: Trend Graph (Dark Color Theme):

![trend graph, dark color theme](/assets/trend_graph_dark.png)

Users can configure custom thresholds for high or low blood sugar alert notifications as well.

### :alarm_clock: Configurable Alerts:

![configurable alerts](/assets/configurable_alerts.png)

### :bangbang: Low Glucose Alert:

![low glucose alert](/assets/low_alert.gif)

## Extension Settings

This extension contributes the following settings:

- `dExtension.enable`: enable/disable this extension
- `dExtension.accountName`: Dexcom account username
- `dExtension.password`: Dexcom account password
- `dExtension.alertsEnabled`: toggle low/high glucose alerts
- `dExtension.urgentLowAlertLevel`: urgent low threshold value
- `dExtension.lowAlertLevel`: low threshold value
- `dExtension.highAlertLevel`: high threshold value
- `dExtension.urgentHighAlertLevel`: urgent high threshold value

## Extension Commands

This extension contributes the following commands:

- `dExtension.fetchAllGlucoseReadingsWithin24Hours`: fetch all glucose readings within the last 24 hours
- `dExtension.clearSessionGlucoseLog`: clear all recorded readings in session storage

## Stack

Developed using the following technologies:

- VS Code Extension API
- Dexcom API
- Chartist.js
- Node.js

<!-- ## Known Issues

- note any known issues here when they are discovered -->

## Feature Pipeline / To-Do

- Refactor to TypeScript
- More robust unit tests
- Modularize utility funcs, refactor main extension logic
- More intelligent error handling / asynchronous flow
- API logic to automate missed reading retrieval and storage
- Export glucose log to CSV
- Configurable chart ranges

## Development Notes / Misc.

- Conceived / developed over the course of four days as a hackathon project
- January 2019 Fullstack Academy Stackathon Award Winner
  - "Mad Science - Most Purely and Absurdly Excellent Project"
- Stackathon Presentation:

  [![thumbnail image for presentation link to YouTube](/assets/youtube_thumbnail.png)](https://www.youtube.com/watch?v=3ITHgLBZaaQ)

## Release Notes

### Pre-Release / Beta

dExtension is still under development and in pre-release as it began as a hackathon project - however, I fully intend to publish it on the Visual Studio marketplace once it is stable enough that other developers with diabetes can download the extension for personal use, so be sure to check back often for release updates!

---

Made with :heart: in NYC by [Scott DeMeo](https://github.com/scottdemeo).
