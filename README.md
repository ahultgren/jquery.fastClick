# jquery.fastClick

Removes the delay between tapping to the click event being sent on iphone and possibly other devices. It's very useful for apps that need to be and feel responsive.

*This code is just passively mantained (aka I will update the code when I need a fix myself). If you use it and feel something is missing/broken, feel free to submit a pull request or create an issue and i might take care of it when I have time.*

Inspiread by some post on HN that i couldn't find again.

## How to use

Minify code by installing grunt and running `grunt`.

```html
<script src="jquery.js"></script>
<script src="dist/fastClick.min.js"></script>
<script>
jQuery(function($) {
  $('a.quick').fastClick(function(e){
    alert('Wrrooooom!');
  });

  $('a.normalButton').click(function(e){
    // Don't abuse .fastClick(). Use normal .click() for normal links where response-time is not critical.
    alert('Zzzzzz...');
  });
});
</script>
```

## License
Copyright (c) 2013 Andreas Hultgren  
Licensed under the MIT, GPL licenses.