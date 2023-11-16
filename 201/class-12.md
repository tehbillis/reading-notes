# Chart.js and Canvas

## Javascript Canvas

The `<canvas>` element lets you draw 2d and sometimes 3d images with javascript.

The closing tag is required and all content between the tags are used as fallback content.

`getContext()` gets the rendering context of the canvas which allows you to draw your shapes.

## JS Canvas Questions

1. **What does the `<canvas>` allow a developer to acheive? -** It allows them to draw 2D images with javascript.
2. **What is the importance of the closing `</canvas>` tag? -** Because `<canvas>` uses the content between the tags as fallback content in case it's not supported by a browser.
3. **Explain what the `getContext()` method does. -** It allows you to get the rendering context for the canvas element. Effectively giving you access to the tools to draw images on the canvas.

## Chart.js

Chart.js is a javascript charting library that uses the `<canvas>` element to create animated and performant charts. It can be installed with npm, included through a CDN, or built from the github repo. You can include the .js file or integrate it with different module loaders.

Chart Types:

* Area Chart
* Bubble Chart
* Doughnut & Pie Charts
* Line Chart
* Mixed Chart Types
* Polar Area Chart
* Radar Chart
* Scatter Chart

## Chart.js Questions

1. **What is Chart.js and how it can be brought into your project? -** A javascript charting library that uses the `<canvas>` element to create animated and performant charts. You can include the .js file, or integrate it with various module loaders.
2. **List 3 different Chart types you can create using Chart.js. -**
   * Area Chart
   * Radar Chart
   * Line Chart

## Animated Charts

This article went over how to setup various chart types with chart.js. It's important to understand how to create a chart and pass data into them. each one follows a similar structure,

```javascript
var buyerData = {
	labels : ["January","February","March","April","May","June"],
	datasets : [
		{
			fillColor : "rgba(172,194,132,0.4)",
			strokeColor : "#ACC26D",
			pointColor : "#fff",
			pointStrokeColor : "#9DB86D",
			data : [203,156,99,251,305,247]
		}
	]
}
```

but each one also had it's own unique setup.

## Animated Charts Questions

1. **What are some advantages to displaying data via a chart over a table? -** They're better at displaying data and they're easier to read.
2. **How could Chart.js aid your previously created applications visually? -**
   * For salmon cookies you could better represent cookie sales with a line chart.
   * For Odd Duck, you can display the product statistics in an easy to digest chart that shows both how many times it was shown and how many times it was selected.

## Things I want to know more about