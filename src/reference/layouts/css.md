# Using CSS

The whole graphic output of a layouts (including the layout elements) are based on [HTML], [CSS] and [JavaScript]. This basically means that create CONFIRE SHOWTIME webites with a special behaviour. 

Even if you position all layout elements via Drag & Drop and can comfortably configure many aspects via the Property Editor you are only controlling a fraction of the graphical possibilities.

If you are using CSS and / or JavaScript as an aid, you can take on every detail of layout elements any influence. For this purpose a small sample:

1. Create a new text element in a layout.

2. Enter some text and set the color, font and background to suit your taste.

3. Now copy the entry under `Referenz-ID` to the Windows clipboard.

4. Open the property editor under `Design > Eigenes CSS` den CSS-Editor.

5. Type in the following CSS Sequence
   
   ```` css
   #text-73D1AECD-1D83-45A9-B421-B5558A2C9DC6 {
      text-shadow: 10px 10px 5px grey
   }
   ````

   Replace the example enter `#text-73D1AECD-1D83-45A9-B421-B5558A2C9DC6` with the newly created Reference-ID.

6. Click on `OK`.

The text in your text element has now got a shadow. How is that possible? Well, you have just deposited a CSS declaration for the HTML element with the ID text-73D1AECD-1D83-45A9-B421-B5558A2C9DC6. And this CSS declaration specifies that a text shadow with a horizontal and vertical offset of 10px, a width of 5px for the Blur and the color to be output gray.

Let's go one step further: Our text with shadow shall now even blink. Replace the existing CSS declaration with this one:

```` css
#text-73D1AECD-1D83-45A9-B421-B5558A2C9DC6 {
   text-shadow: 10px 10px 5px grey;
   -webkit-animation-name: blinker;
   -webkit-animation-duration: 0.5s;
   -webkit-animation-iteration-count: infinite;
   -webkit-animation-timing-function: ease-in-out;
   -webkit-animation-direction: alternate;
}

@-webkit-keyframes blinker {
  from {opacity: 1.0;}
  to {opacity: 0.0;}
}
````

You'll notice now your text flashes now happily to himself.

If you want more, we recommend the following procedure:

1. Brush up on your knowledge of CSS and learn CSS. There are countless launches the web. Simple Search introduction times for the terms `CSS introduction`. A comprehensive reference to CSS can be found at http://www.w3schools.com/css. 

2. Inspect using the HTML structure of the current layout using the Developer Console under `View > Developer Console` (or by pressing `F12`). That's how to get a a better feel for the internal structure of a layout. In addition, you can play around directly with the CSS settings in the developer console. 

3. Think about the effect you would like to implement and try to achieve this with CSS.

Of course even CSS has its limits and as soon as those are reached JavaScript comes into play. With JavaScript you can pretty much achieve all your goals you're then actually using a proper programming language.

[HTML]: ../../simple-glossary.md#html
[CSS]: ../../simple-glossary.md#css
[JavaScript]: ../../simple-glossary.md#js