d3charts is a library that helps you create d3 charts easily. Currently I have only added one chart which is a line area chart. The x axis is only for a date value.

Usage:

include script file:

<script src="d3charts.min.js"></script>

Dependencies:
jQuery
d3
bootstrap (for tooltips)

A chart object can be initialized by the following command:

var lineChart1 = new d3Charts.lineAreaChart({top:30,bottom:50,left:60,
								right:30,width:800,
								height:600,xscale:"months",
								selector:"#graph"});

lineChart1.init(data); 

The variables to be given initially are as follows:

top -- distance of chart from the top margin of svg. Defaults to value 30.
bottom -- distance of chart from the bottom margin of svg. Defaults to value 30.
left -- distance of chart from the left margin of svg. Defaults to value 40.
right -- distance of chart from the right margin of svg. Defaults to value 30.
width -- width of svg. Defaults to value 1200.
height -- height of svg. Defaults to value 600.
xscale -- x-axis date display format. --weeks or months. Defaults to "months".
selector -- container of chart. Defaults to "body".

For updating chart to new values use this command.

lineChart1.update(newData);
