# Layouts

Layouts are the most complex aspect of a CONFIRE SHOWTIME Project. With a layout you determine which layouts via their corresponding scenes will be displayed in a Showcase. 

Layouts are defined hierarchically. At the top of the hierarchy are what's known as Master Layouts which differ from regular layouts in two ways:

* They have no parent layout

* They define the target resolution for themselves and their sublayouts.

The set of layouts forms a tree-like hierarchy:

````
Master Layout
-- Layout 1
   -- Layout 1.1   
   -- Layout 1.2
-- Layout 2
   -- Layout 2.1   
   -- Layout 2.2
-- Layout 3
   -- Layout 3.1   
   -- Layout 3.2
````

On each layout (even on a Master MasterLayout) layout elements can be placed freely. The following layout elements are available:

* Picture Element
* Text Element
* Multimedia Element
* SVG Element
* Website Element
* Panel Element
* App Element

The following aspects of the layout are described in further more detail:

* [Screen Resolutions](multi-resolutions.md)
* [Markdown](markdown.md)
* [Using CSS](css.md)
* [Using RSS](rss.md)
