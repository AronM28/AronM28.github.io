---
layout: post
title: test portfolio
---

This is a test graph for a portfolio taking the html from elsewhere.

Which should appear below.

<<[http://aronm28.github.io/chartjs/test.html]

Or not - how about now?


<script src="http://AronM28.github.io/chart.js/Chart.js"></script>

<div id="canvas-holder">
<canvas id="chart-area" width="400" height="400"/>
</div>

<script>

var doughnutData = [
				{
					value: 25,
					color:"#F7464A",
					highlight: "#FF5A5E",
					label: "UK equity"
				},
				{
					value: 50,
					color: "#46BFBD",
					highlight: "#5AD3D1",
					label: "Green"
				},
				{
					value: 100,
					color: "#FDB45C",
					highlight: "#FFC870",
					label: "Yellow"
				},
				{
					value: 40,
					color: "#949FB1",
					highlight: "#A8B3C5",
					label: "Grey"
				},
				{
					value: 120,
					color: "#4D5360",
					highlight: "#616774",
					label: "Dark Grey"
				}
			];
			window.onload = function(){
				var ctx = document.getElementById("chart-area").getContext("2d");
				window.myDoughnut = new Chart(ctx).Doughnut(doughnutData, {responsive : true});
			};
</script>
