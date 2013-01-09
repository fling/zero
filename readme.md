# zero
zero is a digital starter kit designed to start designing sites and apps quickly.

## Usage
To incorporate zero into your own projects:

* Clone the project into your stylesheets folder.
* Include zero.css into your project using either ```@import``` in your top-level css file or ```link rel="stylesheet"``` in the header of your html.
* Also follow these steps for animate, font-awesome, iscroll, and ronin depending on the features you need.
* Finally, link in ```zero/hacks.css``` the same way after everything else has been included.

For an example, you may consult the zero+1 project, which is a demo/sdk of the this project.

# Components

* reset.css
* layout.css
* controllers.css
	* shelf navigation
	* modal
	* segmentend navigation
	* tabbed views
* buttons.css
* forms.css
* lists.css
* bars.css
* app.css
* flexgrid.css

## reset.css
`reset.css` removes all default styles from all block and inline elements. This is designed to create a true base style on all devices and browsers.

## layout.css
`layout.css` defines the basic layout structure, scrolling and page stack metaphors used in most apps.

	<body class="app">
		<div class="container">
			<div class="stack">
				<div class="card">
				...
				</div>
			</div>
		</div>
	</body>

### scroll
@todo creates a scrollable region

### stack
@todo creates a card stack

### card
@todo defines a card stack

## controllers.css
`controllers.css` defines a variety of controller types:

### shelf navigation
The `#shelf` displays a shelf menu off screen. when active it will push the `.container` to the side and reveal the shelf. tapping anywhere in the `.container` will bring it back into focus.

	<div id="shelf">
	  <div class="clip">
	  	...
	  </div>
	 </div>
	 <a class="mask" href='#' data-unpush="shelf"></a>
	 
When active the `.mask` element creates a definable transparent (or semi-transparent) region to deactivate the control.

### modal
The `.modal` displays a new view over the current `.container` useful for creating new objects, contact forms and other inline tasks.

	<div id="contact" class="modal">
	  <div class="sheet">
	    Something
	  </div>
	</div>
	<a class="mask" href='#' data-unpush="contact"></a>

### segmented navigation
The `.segmented` or `.seg` classes can be used to create  segmented navigation controls, useful for triggering tab views.

	<ul class="seg">
		<li>Alpha</li>
		<li>Bravo</li>
		<li>Charlie</li>
	</ul>

### tabbed views
The `.tabs` displays a more traditional tab controller view.

    <ul class="tabs" data-tabset="tab1">
		<li><a href="#tab1">Tab 1</a></li>
		<li><a href="#tab2">Tab 2</a></li>
		<li><a href="#tab3">Tab 3</a></li>
    </ul>

	<div class="tabs">
		<div id="tab1" class="tab">
			Tab Pane 1
		</div>
		<div id="tab2" class="tab">
			Tab Pane 2
		</div>
		<div id="tab3" class="tab">
			Tab Pane 2
		</div>
	</div>

Adding the `.footer` class to any tabbed menu will position the tabs to the bottom of the screen

	<div class="tabs footer">
		...
	</div>

## buttons.css
@todo

## forms.css
@todo

## list.css
defines a list

### simple list
The most common list

	<ul class="list">
		<li class="header">List Header</li>
		<li>List Item</li>
		<li><a href="#">Linked List Item <i></i></a></li>
		<li><p>A list item with paragraph text.</p></li>
	<ul>

### complex list
when you need more flexibility

	<div class="list">
		<h4>List Header</h4>
		<ul>
			<li>List Item</li>
			<li><a href="#">Linked List Item <i></i></a></li>
			<li><p>A list item with paragraph text.</p></li>
		</ul>
	</div>

### inset list
to create an inset list

	<div class="list inset">
		<h4>List Header</h4>
		<ul>
			<li>List Item</li>
			<li><a href="#">Linked List Item <i></i></a></li>
			<li><p>A list item with paragraph text.</p></li>
		</ul>
	</div>

## bars.css

## app.css
`app.css` 

## flexgrid.css
`flexgrid.css` uses the following markup example to create a flexible layout. Resizing the browser will scale the content up or down to stay reletively purportionate to the screen size.

	<body class="flexgrid">
		<div class="container">
			<section class="content">
			...
			</section>
		</div>
	</body>