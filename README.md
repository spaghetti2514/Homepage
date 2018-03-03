This is a homepage for Webkit and Gecko browsers based on [Ahoka's](https://github.com/ahodesuka) original design, with some added functionality.

Check out the [demo](https://spaghetti2514.github.io/Homepage)


Among its feature are:

- Paged links
- Configurable grid sizes
- Multi-search-engine searching
- A retractable menu
- Hotkeys

# Configuration
To get started configuring, open the config.js file in the js directory.

## Options
The first thing in the config.js file will be several options, each starting with "var" and ending with a semicolon. The option names should be self-explanatory, but each has a comment above it explaining exactly what it does just in case.  
Change the values of these to change various defaults and layouts of your homepage.  

## Search Engines
The next section is for search engines. In each block of options for each search engine, you'll find one called "enabled." Set this to true or false depending on whether or not you want it to be included in the search engine selector.  
Note that bittorrent sites are disabled by default.  

If you have a request for a specific engine to be added, feel free to open an issue on Github

## Menu Links
This section defines the links in the retractable menu. The menu supports an arbitrary number of entries, with the default being 6 (probably). Each entry has a name and url associated with it. The name is what the link will appear as in the menu, and the url is the link's destination. It is recommended that you keep the names short so as not to overflow the menu.  

## Main Links
Here is the portion where the links in the center of the page are defined. Like the retractable menu, each has a name and url to configure.  
You may add more links by duplicating the blocks in the default config, exactly like how entries are added to the retractable menu. Once you have more links than the page can hold (10 by default), another page will be automatically created.  

# Usage

## Retractable menu
The retractable menu is opened by hovering over it, and will close when no longer being hovered over. Clicking on the menu (but not on a link) will keep the menu open even if it not being hovered on.  

## Pages
When multiple pages are present, they can be cycled one of two ways.  
The first way is by using the blue circles at the top of the page. The circle representing the current page will be enlarged, and clicking any other circle will bring you to the corresponding page.  
The second way to cycle pages is by clicking on the far right or left side of the page where the links are. Your cursor should change to reflect the direction clicking will take you.  

## Searching
The search engine can be changed by clicking the selector by the search box and then clicking the desired search engine in the drop-down menu. After typing a query, it can be searched by pressing enter or clicking the submit button with the arrow on it.  

## Hotkeys*
Several hotkeys are defined to make keyboard-use easy.

- The left and right arrow keys will change the current page.
- The up and down arrow keys will extract and retract the menu.
- The number keys (not the numpad [maybe]) can be used to select a specific link on the current page. For example, in a configuration with two rows and five columns, "3" would select the third link in the first row, "7" would select the second link in the second row, and "0" would select the last link.
- The "s" key will change the focus to the search box from anywhere on the page.

*Note that hotkeys are disabled when the search box has focus. If you use them often, it is recommended you change the appropriate setting to not select the search box initially.
