---
layout: post
title: test portfolio
excerpt_separator: <!--more-->
related: ["test", "portfolio"]
---

This is a test graph for a portfolio taking the html from elsewhere.

Which should appear below.

<<[http://aronm28.github.io/chartjs/test.html]

Or not - how about now?

This seems to work okay...

<!--more-->

<script src="http://AronM28.github.io/chart.js/Chart.js"></script>

<div id="canvas-holder">
<canvas id="chart-area" width="400" height="400"/>
</div>

<script>

var doughnutData = [
				{
					value: 8,
					color:"#F44336",
					highlight: "#E57373",
					label: "Property"
				},
				{
					value: 8,
					color: "#673AB7",
					highlight: "#9575CD",
					label: "Emerging markets"
				},
				{
					value: 8,
					color: "#3F51B5",
					highlight: "#7986CB",
					label: "EU ex UK"
				},
				{
					value: 8,
					color: "#009688",
					highlight: "#4DB6AC",
					label: "Japan"
				},
				{
					value: 8,
					color: "#9E9E9E",
					highlight: "#E0E0E0",
					label: "Pacific"
				},
				{
					value: 25,
					color: "#FF9800",
					highlight: "#FFB74D",
					label: "UK"
				},
				{
					value: 35,
					color: "#4CAF50",
					highlight: "#81C784",
					label: "US"
				}
			];
			window.onload = function(){
				var ctx = document.getElementById("chart-area").getContext("2d");
				window.myDoughnut = new Chart(ctx).Doughnut(doughnutData, {responsive : true});
			};
</script>
