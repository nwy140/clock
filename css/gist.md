My own custom digital clock page for use with the Lively Wallpaper open-source app  

## Hackspace Themed
https://nwy140.github.io/clock/index-3.html  

## Ghibli Themed
https://nwy140.github.io/clock/  

## Space Themed
https://nwy140.github.io/clock/index-2.html    

Lively Wallpaper Open-source app  
https://www.microsoft.com/en-us/p/lively-wallpaper/9ntm2qc6qws7?activetab=pivot:overviewtab    
https://rocksdanister.github.io/lively/    


Music Autoplay is disabled by default until the wallpaper is clicked near the bottom edge of the screen    

This repository is a fork of another clock.js repository with some basic digital clock functionality,    
plus some of my own front-end changes    

When previewing on a browser,
for best experience, use a chromium based browser

If a web-app doesn't load properly in Lively Wallpaper  
Install an electron version of that web-app as a desktop app  

https://medium.com/@jordan.eckowitz/make-any-website-into-a-desktop-app-with-1-line-of-code-ba53d59bf9e1  
nativefier --name "Clock-hackerspace" "https://nwy140.github.io/clock/index-3.html"  
  
<!DOCTYPE html>
<html lang="en">
<head>
	<!-- CHARACTER SET -->
	<meta charset="utf-8">

	<!-- VIEWPORT SIZING FOR ALL DEVICES -->
	<meta name="viewport" content="width=device-width, initial-scale=4.0">

	<!-- AUTHOR -->
	<meta name="author" content="Tyler West">

	<!-- DESCRIPTION -->
	<meta name="description" content="A simple digital clock built with html, css, and javascript.  It will give you the time of day in 12 hour format and the day of the week.">

	<!-- TITLE -->
	<title>Digital Clock</title>

	<!-- SHORTCUT ICON -->
	<!-- <link rel="shortcut icon" href="img/favicon.ico"> -->

	<!-- CUSTOM EXTERNAL STYLESHEET -->
	<link rel="stylesheet" href="css/main.css">
</head>
<section class="about-section">

<!-- Start YOutube Background  -->
	<!-- https://codepen.io/dudleystorey/pen/PZyMrd -->
	<!-- https://stackoverflow.com/questions/43691980/youtube-video-as-background-for-webpage -->
	<div class="video-background">
		<div class="video-foreground">
		  <!-- <iframe src="https://www.youtube.com/embed/W0LHTWG-UmQ?controls=0&showinfo=0&rel=0&autoplay=1&loop=1&playlist=W0LHTWG-UmQ" frameborder="0" allowfullscreen></iframe> -->
		  <!-- <iframe src="https://www.youtube.com/embed/a02_GTmBEXY?autoplay=0&showinfo=0&loop=1&list=PL7K_cQ2aVeqn0_3eTOgLMr_4_BN9md4qq&rel=0" frameborder="0" allowfullscreen></iframe> -->
		  <iframe src="https://www.youtube.com/embed/lwLvgvDiyFM?autoplay=1&showinfo=0&loop=1&list=PL7K_cQ2aVeqnHZjPSMRjiMWRWHx5HD_67&rel=0" frameborder="0" allowfullscreen></iframe>

		</div>
	  </div>
	
	<!-- <div id="vidtop-content">
	<div class="vid-info">
		  <h1>YouTube Fullscreen Background Demo</h1>
		  <p>The International Space Station orbits the Earth every 92 minutes, with its crew seeing a sunrise 15 times a day. It exists as a scientific, educational, and engineering platform in low orbit, 330 to 435 kilometres above the Earth.
		 <p>Original timelapse by Riccardo Rossi (ISAA), used under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License. Raw photos courtesy of http://eol.jsc.nasa.gov/
		 <a href="/500/Use-YouTube-Videos-as-Fullscreen-Web-Page-Backgrounds">Full article</a>
	  </div>
	</div> -->
<!-- End YOutube Background -->


<br>
<br>
<br>


<body>


	<div class="date-field">

	<main class="clock-display column">
		<h1 class="myContainer">Clock.js</h1>
		<div class="date-field">
			<div class="day-of-week">
				<p class="day-alpha"></p>
				<p class="placeholder">mmmmmmmmm</p>
				<p class="placeholder">ooooooooo</p>
				<p class="placeholder">nnnnnnnnn</p>
				<p class="placeholder">ttttttttt</p>
				<p class="placeholder">uuuuuuuuu</p>
				<p class="placeholder">eeeeeeeee</p>
				<p class="placeholder">sssssssss</p>
				<p class="placeholder">wwwwwwwww</p>
				<p class="placeholder">hhhhhhhhh</p>
				<p class="placeholder">rrrrrrrrr</p>
				<p class="placeholder">fffffffff</p>
				<p class="placeholder">iiiiiiiii</p>
				<p class="placeholder">ddddddddd</p>
				<p class="placeholder">aaaaaaaaa</p>
				<p class="placeholder">yyyyyyyyy</p>
			</div>
			<div class="day-of-week-mobile">
				<p class="day-alpha-mobile"></p>
				<p class="placeholder">mmm</p>
				<p class="placeholder">ooo</p>
				<p class="placeholder">nnn</p>
				<p class="placeholder">ttt</p>
				<p class="placeholder">uuu</p>
				<p class="placeholder">eee</p>
				<p class="placeholder">sss</p>
				<p class="placeholder">www</p>
				<p class="placeholder">hhh</p>
				<p class="placeholder">rrr</p>
				<p class="placeholder">fff</p>
				<p class="placeholder">iii</p>
			</div>
			<div class="month">
				<p class="month-alpha"></p>
				<p class="placeholder">mmm</p>
				<p class="placeholder">ooo</p>
				<p class="placeholder">nnn</p>
				<p class="placeholder">ttt</p>
				<p class="placeholder">uuu</p>
				<p class="placeholder">eee</p>
				<p class="placeholder">sss</p>
				<p class="placeholder">www</p>
				<p class="placeholder">hhh</p>
				<p class="placeholder">rrr</p>
				<p class="placeholder">fff</p>
				<p class="placeholder">iii</p>
				<p class="placeholder">ddd</p>
				<p class="placeholder">aaa</p>
				<p class="placeholder">yyy</p>
				<p class="type">month</p>
			</div>

			<div class="date">
				<p class="date-number"></p>
				<p class="placeholder">88</p>
				<p class="type">day</p>
			</div>
			<div class="year">
				<p class="year-number"></p>
				<p class="placeholder">8888</p>
				<p class="type">year</p>
			</div>
		</div>
		<div class="clock-field">
			<div class="numbers">
				<p class="hours"></p>
				<p class="placeholder">88</p>
				<p class="type">hour</p>
			</div>
			<div class="colon">
				<p>:</p>
			</div>
			<div class="numbers">
				<p class="minutes"></p>
				<p class="placeholder">88</p>
				<p class="type">minute</p>
			</div>

			<div class="colon">
				<p>:</p>
			</div>
			<div class="numbers">
				<p class="seconds"></p>
				<p class="placeholder">88</p>
				<p class="type">second</p>
			</div>

			<div class="am-pm">
				<div>
					<p class="am">am</p>
				</div>
				
				<div>
					<p class="pm">pm</p>
				</div>

				

			</div>

		</div>

	</main>


	

</div>

<div>


	<p align="center numbers" >
		<!-- https://calendar.google.com/calendar/u/0/embedhelper -->
		<iframe src="https://app.gitkraken.com/glo/board/X97ha7w5GgAS3-0j" style="border:solid 1px #777"
		 width="1500" height="550" frameborder="0" scrolling="no"></iframe>
	</p>
	<p align="right numbers" >
		<!-- https://calendar.google.com/calendar/u/0/embedhelper -->
		<iframe src="https://calendar.google.com/calendar/embed?height=600&amp;wkst=1&amp;bgcolor=%23ffffff&amp;ctz=Asia%2FKuala_Lumpur&amp;src=MDEzMjI5MkBrZHUtb25saW5lLmNvbQ&amp;src=YWRkcmVzc2Jvb2sjY29udGFjdHNAZ3JvdXAudi5jYWxlbmRhci5nb29nbGUuY29t&amp;src=ZW4ubWFsYXlzaWEjaG9saWRheUBncm91cC52LmNhbGVuZGFyLmdvb2dsZS5jb20&amp;src=OTRxcHEzbjA3ZnJrYzhpMGtmN3ZtaXI4dGExMzZtNThAaW1wb3J0LmNhbGVuZGFyLmdvb2dsZS5jb20&amp;src=dDBzYmZ1aGkyZ21tN2x2OHFmOGw1dTZubzY5cG1hcTBAaW1wb3J0LmNhbGVuZGFyLmdvb2dsZS5jb20&amp;color=%23039BE5&amp;color=%2333B679&amp;color=%230B8043&amp;color=%23E67C73&amp;color=%23C0CA33" 
		
		style="-webkit-transform:scale(0.5);-moz-transform-scale(0.5);" 
		width="800" height="600" frameborder="0" scrolling="no" 	></iframe>
	</p>
</div>
`


	<script src="javascript/main.js"></script>
</body>
</html>
dd