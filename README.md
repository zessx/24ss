![24SSgrid](24SSgrid.png)

24SSgrid is a 24-columns solid grid for SASS.

Installation
------------
1. Download the [latest release](https://github.com/zessx/24SSgrid/releases) of 24SS
2. Copy the `scss/24SSgrid.scss` file in your project
3. Add this line to your main SASS file : `@import "24SSgrid";`

Customization
-------------
24SSgrid will still use 24 columns, but you are able to specify two variables, adding thos lines to your main SASS file :

    $gw-column: 30px;
    $gw-gutter: 10px;

Usage
-----
- Use the `.row` class on your wrapper
- Use both `.col` and `.col-x` classes on your columns
- Use `.offset-x` classes to manage empty columns
- You can use nested columns

Example :

    <div class="row">
        <div class="col col-4"></div>
        <div class="col col-18 offset-2">
            <div class="col col-6"></div>
            <div class="col col-6"></div>
            <div class="col col-6"></div>
        </div>
    </div>

Legals
------
- Author : [zessx](https://github.com/zessx)
- Licence : [MIT](http://opensource.org/licenses/MIT) 
- Contact : [@zessx](https://twitter.com/zessx)
- Link  : [http://smarchal.com/24SS/](http://smarchal.com/24SS/)

TODO
----
- 
