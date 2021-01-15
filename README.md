Dead Valley
===========

Escape from Zombie-infested Dead Valley in this HTML5 Grand Theft Auto style Game.

### Running the Game

Opening index.html locally in a browser will not work; you will need to set up a web server. I recommend using [Pow](http://pow.cx/) on a mac. It needs a public directory to host static files so just create a symlink:
```
ln -s . public
```
It's already in the .gitignore file.

### Code

Dead Valley uses [Requirejs](http://requirejs.org/) for code organization.

Required Libraries (Found in *vendor/*)

* [jQuery](http://jquery.com/)
* [Requirejs](http://requirejs.org/)
* [Underscore.js](http://documentcloud.github.com/underscore/)
* [Soundjs](http://www.createjs.com/#!/SoundJS)
* [Modernizr](http://modernizr.com/)

### Editor

The maps are JSON in the *maps/* directory.

There is an HTML5 map editor **editor.html**.
Select tiles on the left, and place them with a click. Free draw with the shift key. The red highlighted tiles in the map are the only places roads should leave the map.

There used to be a way to place full buildings, complete with defined walls and entrances (Building Archetypes) but that seems broken.

### Tests

There's a suite of Jasmine tests in the *test/* directory that put some aspects of the game through their paces. The coverage is spotty and the test code is kind of ratty but at least it exists.

Drag this to your browser bar: <a href="javascript:$.getScript('test/runner.js');">Test Runner Bookmarklet</a>

Reload the game then click on the bookmarklet to run the tests.