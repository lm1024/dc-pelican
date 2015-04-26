layout: post
title: The Worst Metric
author: devcurmudgeon
date: 02/06/2013

Lines Of Code is an awful way to measure software - but look at the pretty picture...

<script type="text/javascript" src="//ajax.googleapis.com/ajax/static/modules/gviz/1.0/chart.js"> {"dataSourceUrl":"//docs.google.com/a/codethink.co.uk/spreadsheet/tq?key=0Aiph3VJv3myMdFBaZTNKUDNFeFVWa3pjY2M3ZlI4dnc&transpose=0&headers=0&range=D2%3AE158&gid=6&pub=1","options":{"titleTextStyle":{"bold":true,"color":"#000","fontSize":16},"animation":{"duration":500},"colors":["#3366CC","#DC3912","#FF9900","#109618","#990099","#0099C6","#DD4477","#66AA00","#B82E2E","#316395","#994499","#22AA99","#AAAA11","#6633CC","#E67300","#8B0707","#651067","#329262","#5574A6","#3B3EAC","#B77322","#16D620","#B91383","#F4359E","#9C5935","#A9C413","#2A778D","#668D1C","#BEA413","#0C5922","#743411"],"theme":"maximized","width":1435,"is3D":false,"pieSliceText":"label","hAxis":{"useFormatFromData":true,"minValue":null,"viewWindow":{"min":null,"max":null},"maxValue":null},"vAxes":[{"useFormatFromData":true,"minValue":null,"viewWindow":{"min":null,"max":null},"maxValue":null},{"useFormatFromData":true,"minValue":null,"viewWindow":{"min":null,"max":null},"maxValue":null}],"pieHole":0,"booleanRole":"certainty","title":"130602 Baserock GENIVI system: approx 32M loc", "height":400, "width":580,"legend":"right","pieSliceTextStyle":{"fontSize":"10"},"tooltip":{}},"state":{},"view":{},"isDefaultVisualization":true,"chartType":"PieChart","chartName":"Chart 2"} </script>
<br/>
That's roughly 32 Million Lines of Code involved in a Baserock [GENIVI](http://www.genivi.org) Baseline Linux system - without any <strike>bloat</strike> <strike>C++</strike> applications. 

Total "effort/cost to develop" would be a much more useful metric generally, but <strike>truthful</strike> accurate numbers are *really* hard to come by, because:

- no-one wants to admit how much they really spent, or how far wrong the original estimates were.
- engineers work on multiple projects simultaneously.
- large-scale projects are done by multiple organisations in "collaboration".
- projects involve 're-use' of deliverables from previous projects, making it hard to measure the new stuff accurately.
- time is billed to 'support', or 'maintenance', or even 'sales' instead of development.

I've never liked COCOMO much - it sucked when we used it in the 80s. And since reading [The Leprechauns of Software Engineering](https://leanpub.com/leprechauns) I'd wager a beer there's no real science under COCOMO, in spite of Barry Boehm's pagecount.

So I'll <strike>get famous when I</strike> launch the devCurmudgeon software analysis suite, to sell with the after-dinner [SCRUM](http://www.devcurmudgeon.com/2010/08/28/software-chaos-ridiculously-under-managed/) lectures. Can't explain the details without an NDA, obviously, but it's a proprietary algorithm involving Git-active-days and the entrails of a chicken.

In the meantime, I'm having to <strike>wing it</strike> analyse using LOC. My <strike>guesses</strike> detailed calculations based on Ohloh's numbers were <strike>ridiculous</strike> questionable, so colleagues suggested [SLOCCount](http://www.dwheeler.com/sloccount/). SLOCCount's numbers are typically smaller than Ohloh's, which is obviously useless when I'm trying to <strike>exaggerate</strike> justify figures for management. SLOCCount appears to be jolly thorough though, and it saves me flipping back and forth on hundreds of web pages.

So, as requested by the program itself, the following data was "generated using David A. Wheeler's 'SLOCCount'". If David (or anyone) can shed light on why SLOCCount sees 10 Million LOC in the Linux kernel, while Ohloh and the rest of the world claim 15, please <strike>sort it out</strike> let me know.

Here's the equivalent picture for the core [Baserock](http://wiki.baserock.org) operating system (approx 25MLOC) on its own.

<script type="text/javascript" src="//ajax.googleapis.com/ajax/static/modules/gviz/1.0/chart.js"> {"dataSourceUrl":"//docs.google.com/a/codethink.co.uk/spreadsheet/tq?key=0Aiph3VJv3myMdFBaZTNKUDNFeFVWa3pjY2M3ZlI4dnc&transpose=0&headers=0&range=D2%3AE55&gid=7&pub=1","options":{"titleTextStyle":{"bold":true,"color":"#000","fontSize":16},"animation":{"duration":500},"colors":["#3366CC","#DC3912","#FF9900","#109618","#990099","#0099C6","#DD4477","#66AA00","#B82E2E","#316395","#994499","#22AA99","#AAAA11","#6633CC","#E67300","#8B0707","#651067","#329262","#5574A6","#3B3EAC","#B77322","#16D620","#B91383","#F4359E","#9C5935","#A9C413","#2A778D","#668D1C","#BEA413","#0C5922","#743411"],"theme":"maximized","width":1435,"is3D":false,"pieSliceText":"label","hAxis":{"useFormatFromData":true,"minValue":null,"viewWindow":{"min":null,"max":null},"maxValue":null},"vAxes":[{"useFormatFromData":true,"minValue":null,"viewWindow":{"min":null,"max":null},"maxValue":null},{"useFormatFromData":true,"minValue":null,"viewWindow":{"min":null,"max":null},"maxValue":null}],"pieHole":0,"title":"130602 Baserock base-system: approx 25M loc","booleanRole":"certainty","pieSliceBorderColor":"#ffffff","width":600, "height":400,"legend":"right","tooltip":{},"pieSliceTextStyle":{"fontSize":"10"}},"state":{},"view":{},"isDefaultVisualization":true,"chartType":"PieChart","chartName":"Chart 1"} </script>