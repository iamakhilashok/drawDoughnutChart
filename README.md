jquery.drawDoughnutChart.js
=================

A SVG doughnut chart with animation and tooltip.
Inspired by Chart.js(http://www.chartjs.org/).

[Demo on my codepen](http://codepen.io/githiro/details/ICfFE)

USAGE
=================
EXAMPLE

[Demo codepen](https://codepen.io/iamakhilashok/pen/GRoWyaW)

Refer the code for data insertion.
Data is gatherd from the "data-plot" attributte its in an array format.


  
        jQuery(document).ready(function() {
            $(".dChart").each(function() {
                var sPlot = $(this).attr("data-plot");
                var sInside = $(this).attr("data-inside");
                var spo = eval(sPlot);

                $(this).drawDoughnutChart(spo, {
                    percentageInnerCutout: sInside,
                    baseColor:"transparent",
					segmentShowStroke:false,
        segmentStrokeWidth : 0
                });
            });
        });

  



Licensed under the MIT License.
