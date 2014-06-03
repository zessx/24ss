![24SSgrid](24SSgrid.png)

24SSgrid is a 24-columns solid grid for SASS.

Installation
------------
1. Download the [latest release](https://github.com/zessx/24SSgrid/releases) of 24SS
2. Copy the `scss/24SSgrid.scss` file in your project
3. Add this line to your main SASS file : `@import "24SSgrid";`

Customization
-------------
You are able to specify a few variables to custom your grid, adding those lines to your main SASS file :

    $sg-nb-column:        24;                   // columns number
    $sg-class-prefix:     '';                   // class prefix
    $sg-column-width:     30px;                 // columns width
    $sg-gutter-width:     10px;                 // space between columns
    $sg-margin-width:     5px;                  // space around rows
    $sg-background-debug: rgba(255, 0, 0, 0.2); // color used to highlight block in debug mode

Usage
-----
- Use the `.row` class on your wrapper
- Use both `.col` and `.col-x` classes on your columns
- Use `.offset-x` classes to manage empty columns
- Use `.break` class to force next column to be on a new line
- You can use nested columns

Example :

    <div class="row">
        <div class="col col-4"></div>
        <div class="col col-18 offset-2 break">
            <div class="col col-6"></div>
            <p class="col col-6"></p>
            <span class="col col-6"></span>
        </div>
        <div class="col col-12"></div>
        <div class="col col-12 break"></div>
    </div>

Debug
-----
You can use the `.debug` class to quickly highlight your grid blocks.   
This class can be used either on an element or on a parent :

    <div class="row">
        <div class="col col-8 debug"></div>
        <div class="col col-8"></div>
        <div class="col col-8"></div>
    </div>
    <div class="row debug">
        <div class="col col-8"></div>
        <div class="col col-8"></div>
        <div class="col col-8"></div>
    </div>

For any reason, you may want to disable the debug mode on a specific element.  
This can be done using the `.no-debug` class :

    <div class="row debug">
        <div class="col col-8 no-debug"></div>
        <div class="col col-8"></div>
        <div class="col col-8"></div>
    </div>

Legals
------
- Author : [zessx](https://github.com/zessx)
- Licence : [MIT](http://opensource.org/licenses/MIT) 
- Contact : [@zessx](https://twitter.com/zessx)
- Link  : [http://24ss.smarchal.com](http://24ss.smarchal.com)

Donations
---------

[![Buy me a coffee !](http://doc.smarchal.com/bmac)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=KTYWBM9HJMMSE&lc=FR&item_name=Buy%20a%20coffee%20to%20zessx%20%28Samuel%20Marchal%29&currency_code=EUR&bn=PP%2dDonationsBF%3abmac%3aNonHosted)
				
TODO
----
- Add fluid grid
- Find a way to avoid `.break` usage
