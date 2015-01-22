---
layout: page
title: test
---

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris a feugiat justo. Nulla rutrum, enim non commodo posuere, libero dui ullamcorper risus, eu sagittis ex neque vitae purus. Donec lobortis lorem non dapibus luctus. Quisque feugiat, risus eget finibus tincidunt, lacus magna pharetra mauris, finibus consectetur dui felis at ligula. Praesent placerat feugiat massa, eu luctus metus convallis vel. Phasellus id urna euismod, tempus nisi sed, tristique felis. Cras tristique mollis neque vel posuere. Cras sit amet tincidunt dui, quis condimentum erat. Pellentesque nisi mi, commodo id tempus ac, viverra eget ipsum. Cras in ante justo. Aliquam at congue tortor. Mauris vel eleifend orci.

Thanks for visiting.





<script src="http://AronM28.github.io/chart.js/Chart.js"></script>

<div id="canvas-holder">
<canvas id="chart-area" width="300" height="300"/>
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