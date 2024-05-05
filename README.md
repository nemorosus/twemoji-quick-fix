# twemoji-quick-fix
For junkies wanting a quick fix and get that good, sweet Twitter Emojis on their site asap. Dirty way, of course.

Just before you close your </head> tag, copy-paste this code:

```
<script src="https://cdn.jsdelivr.net/npm/@twemoji/api@latest/dist/twemoji.min.js"
crossorigin="anonymous"></script>

<script>
  window.onload = function() {    
    // Parses the document body and    
    // inserts <img> tags in place of Unicode Emojis    
    twemoji.parse(document.body, 
                  {folder: 'svg', ext: '.svg'} // This is to specify to Twemoji to use SVGs and not PNGs
                 );

  }
</script>
```
It should work. This gives you beautiful flags even on Windows, so, yeah. Recommended. Reverse-engineer the links to find more about configuration, because I have no freaking clue where I found this hah. Enjoy!
