HaxePunk CHANGELOG

v2.4.1
------------------------------
* [XXLTomate] Option to play an emitter animation backwards 
* [XXLTomate] Fix invisible particles
* [kpaekn] Added Image.smooth getter and setter
* [ibilon] Smooth for non-flash target
* [ibilon] Fix doc generation script
* Update for new version of openfl

v2.4.0
------------------------------
* Speed improvements for openfl-bitfive
* Template improved to match asset folder names
* [fserb] Added ImageMask
* [XXLTomate] Added pause/resume function to Graphic
* [ibilon] Fix key mapping on native
* [ibilon] Tilemap and Canvas can be scaled
* Fix Flash memory leak (multitouch)
* [ibilon] Nameless images can be flipped
* [kpaekn] scaled images were not flipped correctly on native
* [ibilon] Image can take BitmapData on native
* [ibilon] Sound wouldn't stop at end on native
* [ibilon] Backdrop rendered one too many rows/columns
* Added Ouya controller mapping
* [ibilon] Trace capture is now optional for console
* [fserb] Fix canvas rendering on native
* [fserb] Tilemap rendering fixes
* [ibilon] destroy old graphic when changed
* [ibilon] Text alpha rendering fix
* Several additions from FlashPunk
* Improved documentation

v2.3.2
------------------------------
* [ibilon] Fix circle/grid collision
* [ibilon] Fix grid debug overlay
* [ibilon] Fix moveAtAngle
* [elnabo] Fix Tilemap/Grid load from array

v2.3.1
------------------------------
* [ibilon] Changed render mode to BUFFER for HTML5
* Matching OpenFL 2x2 matrix ordering change in 1.0.2
* [elnabo] Fixed/added load from array for Tilemap and Grid
* [ibilon] Allow setHitboxTo for all targets
* Allow renderMode to be set in Engine constructor
* Fixed seamless Sfx looping on native targets
* Added Xbox button configuration for Mac
* Fixing flipped images when angle != 0
* Changed joystick axis to start at 0 instead of 1

v2.3.0
------------------------------
* Adding OpenFL support
* [julsam] Xbox controller support
* [MaskedPixel] Improved scaling, atlas layer management
* [MALHCat] apply parent position to image render
* [squiddingme] spritemaps animate the same in fixed timestep mode
* Fixed Tilemap usePositions for native rendering
* Added HXP.fullscreen to toggle between windowed and fullscreen modes
* Various fixes from FlashPunk

v2.2.1
------------------------------
* (Native) Draw working on hardware targets
* (Native) PreRotation frameAngle renders correctly
* (Native) Image scale and origin matches Flash
* (Native) Added support for Emitter frames
* [XXLTomate] Fixed upper/lower case input
* [MaskedPixel] Fixed width/height for Image/Text
* [MaskedPixel] Fixed ghost text in Flash
* [thecodethinker] Added a cross method to Vector
* [DjPale] Check that scene exists in onCamera
* [julsam] Fix debug renderEntities when entity's scroll is != 1
* [julsam] Allow Draw.line() to draw out of the screen boundaries
* [XXLTomate] fixed memory leak for non flash targets
* (Native) Fixed Text.color
* [MaskedPixel] World.camera should be favored over HXP.camera

v2.2.0
------------------------------
* [raistlin] Ready for Haxe 3 and Neko 2
* PreRotation no longer throws null error on Flash
* HXP.RAD and HXP.DEG cause angles to spin the same on all targets
* Fixed tearing issues with scaled Tilemaps
* Fixed Text not showing and scaled position
* Added HXP.orientations to restrict orientation modes on mobile devices
* Debug draw for Grid looks correct in scaled scenes
* Atlases share rendering data for identical images
* [FlashPunk] Added filtered volume/pan to Sfx

v2.1.1
------------------------------
* [stevedecoded] Added Entity.moveAtAngle
* [nadako] Fixed Scene not working (World officially deprecated)
* Improved Atlas memory management

v2.1.0
------------------------------
* Major performance improvements on native targets
* Text is hardware accelerated
* Hardware acceleration is turned on automatically for every graphic class
* Renamed World to Scene (although World still exists as a wrapper)
* Multitouch support
* Added Atlas functions (destroy, destroyAll, count)
* [scriptorum] Updated keycodes for NME 3.5.5
* [YAYitsAndrew] Fixed image scaling factor
* [YAYitsAndrew] added HXP.alarm and delay support to HXP.tween
* Fixed console watch order
* Added default HaxePunk icon for new projects
* Image.createRect and Image.createCircle work on all targets

v2.0.3
------------------------------
* Added clipping to Atlas regions
* Added drawCallThreshold and smooth variables to Atlas (improves rendering)

v2.0.2
------------------------------
* Bug fixes for x/y scaling values
* World.getClass handles any input class (for interfaces)

v2.0.1
------------------------------
* Fixed Tilemap rendering when camera moves (cpp/neko)
* Initializing _count in Masklist to prevent neko crash
* [AndyLi] Correctly resize the source of Text

v2.0.0
------------------------------
* Hardware acceleration using TextureAtlas and the display list
* [DelishusCake] moveBy now checks moveCollideX/Y before moving

v1.7.2
------------------------------
* [MattTuttle] Improved joystick support (multiple axis, pressed/checked buttons)
* [MaskedPixel] Fixed inline HXP.colorLerp on native targets
* [MattTuttle] Updated to work with NME 3.5.x
* [Lythom|MattTuttle] Added mouseWheelDelta and mouseCursor to Input class
* [MattTuttle] Fixed drawToScreen when blendMode is null
* [MattTuttle] Reorganized template assets folder

v1.7.1
------------------------------
* Get mouseX/mouseY correctly even when FP.screen is translated/rotated
* Enforce frame index to stay within frame count boundaries
* Refactor FP.approach and FP.clamp to return sooner
* Prevent multiline Text objects from having final line cut off
* [MattTuttle] Masklist supports Circle/Polygon and debugDraw
* [MaskedPixel] fixed infinite loop when calling removeTween on the same tween

v1.7.0
------------------------------
* [Lythom] world.collidePoint returns the topmost entity
* [YAYitsAndrew] Tween.cancel added from FlashPunk
* [zlumer/MattTuttle] Tween handles events (start, update, finish)
* [MaskedPixel] Image originX/Y corrected to match FlashPunk
* [MattTuttle/tangzero] Improved template creation (haxelib run HaxePunk new ...)
* [MaskedPixel] Merged several changes from FlashPunk to HaxePunk
* [MattTuttle] haxelib uses include.nmml file
* [MattTuttle] addGraphic no longer creates a list when graphic=null
* [MattTuttle] console can be removed entirely from a build

v1.6.7
------------------------------
* [jgroeneveld] HXP.tween fix for native targets
* [jgroeneveld] Fixed spritemap for native targets
* [andyli] API improvements and for loop optimizations
* [MaskedPixel] Fixed entities missing world reference when remove called
* [MaskedPixel] Entity can have instance names
* Added a new preloader, requires gfx/preloader folder

v1.6.6
------------------------------
* Entity.addGraphic now correctly adds the new graphic if a list is created
* Fixed text resizing when wordwrap is true and resizable is false
* Removed automatic extensions from Sfx class
* VarTween and MultiVarTween now support properties
* Fixed more initialization errors in neko

v1.6.5
------------------------------
* Improved console output (memory usage, handles properties, terminal output)
* Added HXP.round for rounding to the nearest decimal
* Added width/height to Stamp [mkosler]

v1.6.4
------------------------------
* Fixed black background on Text graphics
* Updated Text class with extra options
* scaleHeight in Entity is now scaledHeight
* Console draws properly when window resizes
* Added global tweener
* Functions added for focus gained/lost
* Added Draw.text
* Fixed several neko bugs

v1.6.3
------------------------------
* bug fixes to Circle/Mask collision
* setHitboxTo now properly sets the entity dimensions
* improved examples
* removed unnecessary property getter/setter functions
* general code cleanup

v1.6.2
------------------------------
* [MarekkPie] moveBy/moveTowards can now handle Array<String> as well as String values.
* added version info to first line of the console log
* Tilemap constructor now handles asset strings
* added platformer example project
* fixed several neko crash bugs (initialize to zero)
* Image.createRect fixed so it no longer creates a transparent image
* fixed circle-circle collision
* improved BitmapData size restrictions for flash10

v1.6.1
------------------------------
* Fixed compilation errors for neko and html5 targets
* Changed grid to use a boolean array instead of BitmapData
* Added HXP.createBitmap to handle BitmapData creation. It checks dimensions and converts the color format in neko
* Minor adjustments to build.xml to ease development
* Fixed flash.Capabilities compile error for html5 target

v1.6.0
------------------------------
* Screen can now be resized. This is done by destroying the BitmapData buffer object and recreating it.
* Fixed several crash bugs in cpp targets

v1.5.0
------------------------------
* Initial port
