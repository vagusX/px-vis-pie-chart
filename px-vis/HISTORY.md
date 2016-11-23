v0.6.45
==================
* updating slider dependency

v0.6.44
==================
* changing all devDeps to ^

v0.6.43
==================
* Update dependency versions

v0.6.42
==================
* Update px-theme to 2.0.1 and update test fixtures
* added xlink namespace to svg

v0.6.41
==================
* updated link inside px-vis to correct link (was missing path)

v0.6.40
==================
* changed radial scale to use infinity instead of max and min number
* added if statement for line canvas to check if chartData and axes are present
* updated px-vis html with all components

v0.6.39
==================
* fixed bug in IE when starting an svg line with mutedSeries

v0.6.38
==================
* fixed axis tickFormat check so it looks for function, not object

v0.6.37
==================
* fixed for event icons and clip path; changed how redrawing event icons works
* added check to ensure that dates from currentDomain is valid for brush
* fixed isObjEmpty check so it also checks for null

v0.6.36
==================
* fixed axis ticks setting when it is only an object
* added ability for axis tickFormat to be an object

v0.6.35
==================
* removing px-theme style call

v0.6.34
==================
* changing Gruntfile.js to gulpfile.js

v0.6.33
==================
* added additional check to brush zoomBrush
* fixed attrs in tooltip being passed down to register
* created chart behaviors for axisConfigs and registerConfigs
* doc fixes

v0.6.32
==================
* added more checks to event and axis mutedSeries bars
* fix to scale extents where chart data ys do not share an x
* added more math.max checks for sizing
* fix to navigator brush so it cannot disappear when fully collapsed
* added more checks on zoomBrush for onload
* added check on axis bar draw to see if it is in mutedSeries
* check mutedSeries observer in axis to only run if titles exist.
* added check to make sure the register elem clicked on has a name, otherwise transverses path to find it
* Added check for currentDomainX & currentDomainY for event draw
* Enable event deletion
* Fix in interaction space to ensure removal of mousemove event
* Fix to allow axes to delete from radar chart

v0.6.31
==================
* bower updating px-demo-snippet

v0.6.30
==================
* Fix intermittent bug in IE when drawing an image on a canvas withing an image load
* Added timeData to px-vis-interaction-space so that non time based charts can use forceDateTimeDisplay on their register/tooltip

v0.6.29
==================
* IE min-height + flex bug fix for register / tooltip

v0.6.28
==================
* increased register height for scrollbars

v0.6.27
==================
* fix for large number of series in register
* fix series bars on chart navigator axis
* fix bug where deleting a series does not update mutedSeries and register

v0.6.26
==================
* added check that actionArea box has a selection
* fixed empty seriesKeys with backwards compatibility
* set chartExtents on range change to fix resize
* included radial definition in axis brush

v0.6.25
==================
* removed extra {

v0.6.24
==================
* fixed merge conflict

v0.6.23
==================
* added check for chartData being undefined in chartCommon

v0.6.22
==================
* fixed completeSeriesConfig generation for mins and maxes
* added checks for d3 selection existance
* changed clip path declaration
* better fixed linePath/lineGroup not being defined on detach

v0.6.21
==================
* Added PxVisBehaviorChart.registerPositioning behavior to avoid code duplication
* Allow interaction space action box to be drawn with mouse outside of interaction space
* prevent errors when releasing mouse button on interaction space when the click had started outside of it
* Call notifyResize when preventResize becomes false

v0.6.20
==================
* fixed chartExtents running prematurely
* fixed linePath not being defined on detach

v0.6.19
==================
* fixed bug with range moment conversion
* added check to scale for x and y before selectedDomain

v0.6.18
==================
* moved polyfills into its own file
* fixed on-hover when chart all data is removed
* set extents to range when available to avoid race condition on selectedDomain and chartExtents
* pass seriesKeys to interaction space to remove registers on all data removed
* added 0 check to width and height in interaction space
* changed data converter to return empty dataset if originalData is empty

v0.6.17
==================
* make sure progressive rendering doesn't "break" the line between batches
* ensure datasets with 5 or less points still render when progressive rendering is on

v0.6.16
==================
* included includes polyfill for IE11

v0.6.15
==================
* bug fix for radial scale
* fixed useDegrees for line
* misc other bug fixes
* fixed register with 0 value
* changes to README
* bug fixes for brush to prevent negative values
* added various truthy tests for 0 values throughout
* fix for register with value = 0

v0.6.14
==================
* fix registers for pie
* moved forcedatetimedisplay to behavior
* general bug fixes for register

v0.6.13
==================
* added delaying chart draw until attached

v0.6.12
==================
* added additional check to radial scale

v0.6.11
==================
* changes for demo

v0.6.10
==================
* make sure scatter removes on detached

v0.6.9
==================
* ensure forceDateTimeDisplay works with new registers

v0.6.8
==================
* fix typo that would break the navigator series drawing

v0.6.7
==================
* make sure addition/removal of series to seriesConfig are correctly processed

v0.6.6
==================
* Added datetime imports to tooltip and passed down to register

v0.6.5
==================
* Made tooltip detach px-tooltip

v0.6.4
==================
* Updated docs across all components

v0.6.3
==================
* ensure brushing works when resizing

v0.6.2
==================
* added rect clip path for canvas
* update docs

v0.6.1
==================
* ensure brush initializes
* ensure multi axis passes the font size down

v0.6.0
==================
* exposed number formatting in register and tooltip
* changed opacity on hover in scatter-radial
* fixed axis series bar opacity on drawing
* fixed muting a series with a '.' in the id when clicking register
* fixed d3 console errors
* refactored navigator initialization
* exclude 'null' data point from line and scatter
* added clip path to canvas
* fixed bugs with the new register
* fixed area clip path to work with iron resize

v0.5.13
==================
* Merged reigster refactor

v0.5.12
==================
* Fixed vis demo
* all demos and demo snippets are up to date and working
* added codepen links

v0.5.11
==================
* draw max value in radial gridlines

v0.5.10
==================
* redraw axis on tick change

v0.5.9
==================
* make sure we observe seriesId for dynamic properties

v0.5.8
==================
* added ability to set domain with radial scale
* added limit radius to radial line
* fixed brushing with raidal axes
* added behavior for dynamically watching properties tied to completeSeriesConfig
* fixed how we expose some properties in completeSeriesConfig
* bug fixing

v0.5.7
==================
* scale now notifies on x axis creation
* move polarData behavior to common
* fix demo

v0.5.6
==================
* Adding offset in series clippath
* Fix padding on axis series bar title
* Fix axis title not redrawn on resize

v0.5.5
==================
* Fix register mutedSeries when ID has a '.'
* Changed series config in chart behavior so it doesnt require x and y

v0.5.4
==================
* Fix for reordering axes on radial with 3 axes

v0.5.3
==================
* exposed mutedOpacity in seriesConfig and ensure muting wors in all scenarios (canvas, svg, progressive rendering...)

v0.5.2
==================
* fixed ordinal data parsing

v0.5.1
==================
* Fixed navigator line

v0.5.0
==================
* Added support for radial charts (polar chart and radar chart)
* Separated line into svg and canvas lines
* Various bug fixes
* Various new features
* Improved demos

v0.4.8
==================
* fixed vulcanized spelling mistake in ghp

v0.4.7
==================
* removed extra demo link in the ghp script

v0.4.6
==================
* adding polygit imports for codepen

v0.4.5
==================
* adding check for Px.d3

v0.4.3
==================
* fixing px-d3 issue

v0.4.2
==================
* added check to parse JSON for configuration objects

v0.4.0
==================
* Converted to Gulp

v0.3.15
==================
* fixed errors when muting all axes

v0.3.14
==================
* add check for data in line

v0.3.13
==================
* added notify true to mouseRect in interaction space

v0.3.12
==================
* added deleteAllBrushes method to axis brush

v0.3.11
==================
* added check in axis brush for chartData

v0.3.10
==================
* added units to data converter series config

v0.3.9
==================
* fixed tests

v0.3.8
==================
* tooltip design fixes
* fixed brushes with muting and unmuting

v0.3.7
==================
* changed default date format to 24hour clock

v0.3.6
==================
* fixed axis label format so it can accept linear or time
* added am/pm to default time format
* update axis tests

v0.3.5
==================
* fixed margin in multi axis

v0.3.4
==================
* fixing NaN on axis issue

v0.3.2
==================
* fixed data converter with empty datasets

v0.3.1
==================
* changed tooltip targets in multi axis

v0.3.0
==================
* tooltip now uses px-tooltip
* associated changes to support that

v0.2.7
==================
* modified grid so it can remove itself on detach

v0.2.6
==================
* added to data converter so it outputs a set of empty datasets

v0.2.5
==================
* fixed maintaining axis brushes on data change

v0.2.4
==================
* fixed title rotation when id has a .

v0.2.3
==================
* added axis brush update on domainchange

v0.2.2
==================
* fixed tests for safari 8

v0.2.1
==================
* fixed tests

v0.2.0
==================
* Large refactor to deal with many timing issues and other bug fixes

v0.1.33
==================
* Fix 'contains' issue on IE for label tooltip

v0.1.32
==================
* multiaxis mouse listeners
* update tests

v0.1.31
==================
* clears an axis brush if that axis is removed

v0.1.30
==================
* mute / unmute issues
* changed the axis id
* enabled redraw of chart through removing data
* events fire on progressive rendering
* added px-tooltip on axis label
* enabled min size to axis brush
* fixed font issues
* fixed axis brush color

v0.1.29
==================
* fixed bug with axes brush and new axes
* fixed grid alignment issues
* enabled axis name in series config

v0.1.28
==================
* documentation updates

v0.1.27
==================
* Fixing multi scale issue on adding axes through chart data

v0.1.26
==================
* Many changes associated with enabling mute / unmute on parallel coords

v0.1.25
==================
* Added support for units in axis labels

v0.1.24
==================
* Fixed bug in axis brush where the array declaration is wrong

v0.1.23
==================
* Adding truncation to axis labels

v0.1.22
==================
* Make sure progressive rendering is cancelled on new drawing request

v0.1.21
==================
* Added preventResize option for chart auto resize.
* Added option to prevent progressive rendering for canvas (preventCanvasProgressiveRendering)
* Make export to png dynamically choose between native and canvg (hence fixing it on edge)

v0.1.20
==================
* Fix bug in empty navigator

v0.1.19
==================
* Fixing color issue in pie

v0.1.18
==================
* Adding support to export chart components to images

v0.1.17
==================
* Fix missing type in px-vis-pie _arcs

v0.1.16
==================
* Allow chart navigator to be used without data and/or driven by a "range" attribute

v0.1.15
==================
* Fix racing conditions with rangepicker

v0.1.14
==================
* Make sure rangepicker can be used in combination with time based charts

v0.1.13
==================
* Fix brush and axis-brush for dynamic sizing

v0.1.12
==================
* auto resize on chart navigator

v0.1.11
==================
* bug fixes, progressive rendering for canvas

v0.1.10
==================
* bug fix

v0.1.9
==================
* Improving tests and bug fixes

v0.1.8
==================
* Make auto resize work for multi axis/scale/brush

v0.1.7
==================
* Added demo link to README

v0.1.6
==================
* Improve data handling by pie slices, allow empty data as well

v0.1.5
==================
* Added vulcanize index and demo

v0.1.4
==================
* fixed navSeriesLimit in navigator

v0.1.3
==================
* improve pie transitioning

v0.1.2
==================
* Fixed line seriesID bug

v0.1.1
==================
* Upgraded navigator to add precipitationPattern behavior

v0.1.0
==================
* Added canvas support: canvas element and ability to render lines to canvas.
* Added ability to gives lines a gradient opacity.

v0.0.7
==================
* Fix tooltip positioning

v0.0.6
==================
* fix positioning for pies

v0.0.5
==================
* behavior documentation fixes

v0.0.4
==================
* Fixed tooltip demo

v0.0.1
==================
* Initial release
