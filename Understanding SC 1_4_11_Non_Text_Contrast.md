SC 1.4.11 covers non-text contrast aspects including the visual indication of focus

##How the criterion relates to focus indication
###What it does not do
* does not specify a size, location, or style of the focus indicator
* does not address contrast difference betwen focused and unfocused states

===What it does do
* Requires contrast wtih adjacent colors

==Core principles
Note: The border is the edge of the component.  An outline property that has 0 or positive values is considred to be outside the component.
* if the indicator is outset from the component, compare against adjacent colors of the background outside the component
* If the indicator is inset, compare against the component background
* If the indicator is the border of the component, compare against both the adjacent compo9nent and page background colors
* If the indicator strattles both inside and outside the component you can choose to meet either adjacent contrast of the page backgroudn or the component background
* Default browser indicator passes only if you hve not modified any style aspects of the component.
** Once you modify style aspects of a component then you can't rely on the default indicator as safe harbor

==Testing
* Use the developer tools to what is used for focus state and where it is placed (e.g. look at outline property and offset)
** Extensions such as Stylus can be used apply or remove styles from outline and border if you are not able to interpret dev tools
* Use a contrast tool to compare the adjacent colors
* If the indicator is a gradient or shadow only enough of it needs to contrast - not the whole indicator as there is no size requirement
