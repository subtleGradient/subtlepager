subtlePager
===========
Super Simple Javascript Paging System
-------------------------------------

#### by **Thomas Aylott** aka *oblivious at subtleGradient.com*

----

## How does it work?

First, include all your html on the page. Give each paged element a classname of `page1`, `page2`, etc... as many as there are. Then add the classnames `subtlePager` `page1` and `pages10` to the parent element. You can have unlimited pagers per page. See the `subtlePager.demo.html` file for a working demo.

### Setup

* HTML
	* **[required]** Parent element
		* `id` attribute
		* `class` attribute  
		EG: `subtlePager pages5 page1`
			* `subtlePager`  
			This classname is required by the default CSS
			* `pages#`  
			`#` is the maximum number of pages, EG: `pages5` for a total of 5 pages
			* `page#`  
			`#` is the default page to display. I recommend just using `page1` here
	* **[required]** Child elements
		* `class` attribute
			* `page#`  
			`#` is the page number that you want this element to be visible on.
	* **[required]** Trigger element(s)
		* **[optional]** `onclick`
			* `subtlePager.page(elementId)`  
			* `subtlePager.page(elementId, true)`  
			* `subtlePager.page(elementId, 5)`  
			
* CSS
	* **[optional]** Define your custom *"CSS Static Logic"*
* JS
	* **[optional]** Redefine defaults

You'll need to attach the functions to your trigger elements somehow, the simplest method is to just use an `onclick` attribute. But I highly recommend you use an eventListener somehow. I leave that as an exercise for the reader.


### Triggering Functions

`subtlePager.page(elementId)`  
Goes to the previous page

`subtlePager.page(elementId, true)`  
Goes to the next page

`subtlePager.page(elementId, 5)`  
Goes to page 5

----

### The MIT License

Copyright (c) 2008 Thomas Aylott

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
