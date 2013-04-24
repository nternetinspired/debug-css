# debug.css – v1.0

Debug CSS is a small, standalone, stylesheet to help visually identify invalid and potentially inaccessible markup, *during development*.

It based entirely upon a portion of the excellent [inuit.css](https://github.com/csswizardry/inuit.css/) (a powerful little framework designed for _serious_ developers) by [Harry Roberts](https://github.com/csswizardry), and all credit should go to him.

I simply broke out Inuit's _debug.scss and implemented it as a stand-alone stylesheet so that it can be quickly and easily linked to from any project to aid in fast visual debugging.

**Usage**

Simply include a link to the stylesheet in the head (i.e. before the </head>) of your document, like so:

    <link href="https://rawgithub.com/nternetinspired/debug-css/master/debug.css" media="all" rel="stylesheet" type="text/css" />

Or create a new bookmark and copy the following code into the URL field to create a bookmarklet to quickly debug any page:

    javascript:(function(){var e=document.createElement("link");e.setAttribute("href","https://rawgithub.com/nternetinspired/debug-css/master/debug.css");e.setAttribute("rel","stylesheet");e.setAttribute("type","text/css");e.setAttribute("media","all");document.head.appendChild(e)})();

If there are potential issues, you'll see some more colour on your site:

 * Red          ==      definite error
 * Yellow       ==      double-check

You can then simply check with your browser tools to see why that colour style is being applied.

**Heads up: Don't forget to remove the link to debug.css once you've finished debugging.**

## Credits

Credit should go to [inuit.css](https://github.com/csswizardry/inuit.css/) creator, [Harry Roberts](https://github.com/csswizardry) for the original _debug.scss in that framework.

Thanks also to [@pjkix](https://github.com/pjkix) for adding the bookmarklet above.

## License

Copyright 2013 Seth Warburton

Licensed under the Apache License, Version 2.0.

---
