jquery-progresstracker
======================

A small (2KB) jQuery plugin that creates a fixed progress indicator based on your content and allows linking between them.


Linking - default: true
When set to true, clicking on a bullet will animate to the top of that section on the page

tooltip - default: “constant”
This determines when the tooltip for a bullet should be shown. There are 2 options:
• “constant” - The active tooltip is always shown, and change as you move between sections. No other tooltip is visible at any point.
• “hover” - As standard all tooltips are hidden, but when you hover a bullet, the tooltip for that one appears.

positiveTolerance - default: 0
Integer - The number specified is added to the default value at which the tracker changes to the next section. For example, if the next section started at 200px, and a positiveTolerance of 50 was specified, the tracker would not switch to the next section at 250px.

negativeTolerance - default: 0
Integer - The number specified is subtracted from the default value at which the tracker changes to the next section. For example, if the next section started at 200px, and a negativeTolerance of 50 was specified, the tracker would not switch to the next section at 150px.

displayWhenActive - default: true
Only displays the progress tracker when the user is between the top of the first section and the bottom of the last; essentially, it is only shown when the tracker sections are in view. Specify false if you want the tracker to always show.

disableBelow - default: 0
Integer - Specify the value (in pixels) that you wish the progress tracker to be hidden when it is below that.

tracking - default: “tracker”
Specifies what the plugin takes into account when deciding when to switch to the next section.
• “tracker” - With this specified, the tracker will switch to the next section when the top of the tracker element is in line or below the threshold of that section (the demo has this behaviour)
• “viewport” - Instead of being based on the top offset of the tracker, this option switches the tracker’s active section when that section reaches the top of the viewport (window)