---
layout: post
title: test portfolio
---

This is a test graph for a portfolio taking the html from elsewhere.

Which should appear below.

<<[http://aronm28.github.io/chartjs/test.html]

Or not - how about now?

This seems to work okay...

<script src="http://AronM28.github.io/chart.js/Chart.js"></script>

<div id="canvas-holder">
<canvas id="chart-area" width="400" height="400"/>
</div>

<script>

var doughnutData = [
				{
					value: 8,
					color:"#F7464A",
					highlight: "#FF5A5E",
					label: "Property"
				},
				{
					value: 8,
					color: "#46BFBD",
					highlight: "#5AD3D1",
					label: "Emerging markets"
				},
				{
					value: 8,
					color: "#FDB45C",
					highlight: "#FFC870",
					label: "EU ex UK"
				},
				{
					value: 8,
					color: "#949FB1",
					highlight: "#A8B3C5",
					label: "Japany"
				},
				{
					value: 8,
					color: "#4D5360",
					highlight: "#616774",
					label: "Pacific"
				},
				{
					value: 25,
					color: "#00A9FF",
					highlight: "33BAFF",
					label: "UK"
				},
				{
					value: 35,
					color: "#BA8BAF",
					highlight: "#C49BBA",
					label: "US"
				}
			];
			window.onload = function(){
				var ctx = document.getElementById("chart-area").getContext("2d");
				window.myDoughnut = new Chart(ctx).Doughnut(doughnutData, {responsive : true});
			};
</script>
