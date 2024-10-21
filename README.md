# p5play template

This is a template repo that includes the following libraries:

* [p5 & p5.sound](https://p5js.org/download/)
* [p5play & planck](https://github.com/quinton-ashley/p5play)

See the links for license information.

`sketch.js` has a very simple game to demonstrate a few features of the p5play library. (Since it's hosted via GitHub Pages, you can [play it here](https://fsudigitalmedia.github.io/p5play_template/)). Wipe it out and make your own game! (After you record your high score, of course.)

## Q5.js

The creator of p5play has created an alternative to p5.js called [q5.js](https://q5js.org/). It is smaller, faster, and better at some things than p5. Maybe that matters to you or maybe it doesn't. The p5play vscode extension (which is very useful) uses q5 by default so it's worth knowing something about it.

If you copy and paste the code from this repo's sketch.js file, you'll see that it breaks. I'm not totally sure why, but it seems to require replacing `let canvas = new Canvas("fullscreen")` with `createCanvas("fullscreen")`. Otherwise, it works.

One other detail is that the `textFont()` function in q5 doesn't accept the font size as a second parameter, so you'll want to specify the font and the size separately:

```javascript
    textFont("Courier");
    textSize(24);
```

## Notes

If you want to include sound, be sure to uncomment the line in `index.html` that includes the `p5.sound` library. (It's worth noting that q5.js still uses the p5 sound library)

Finally, if you're using this as a template, change the title in `index.html` and replace the contents of this `README.md` file with information about the game you've created.
