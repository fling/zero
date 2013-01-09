# zero
zero is a digital starter kit designed to start designing sites and apps quickly.

## Usage
To incorporate zero into your own projects:

* Clone the project into your stylesheets folder.
* Include zero.css into your project using either ```@import``` in your top-level css file or ```link rel="stylesheet"``` in the header of your html.
* Also follow these steps for animate, font-awesome, iscroll, and ronin depending on the features you need.
* Finally, link in ```zero/hacks.css``` the same way after everything else has been included.

For an example, you may consult the zero+1 project, which is a demo/sdk of the this project.

### Apps

### Flexible Grid Layouts
Example markup template for a layout using the flexible grid. Resizing the browser will scale the text up or down to stay purportionate to the screen size.

	<!doctype html>
	<html lang="en">
	<head>
		<meta charset="utf-8">
		<title>Title</title>
		...
	</head>
	
	<!-- specify the layout type -->
	<body class="flexgrid">
	<div class="container">

		<section class="content">
		...
		</section>

	</div>
	</body>
	</html>