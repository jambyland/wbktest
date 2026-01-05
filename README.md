boilerplate intellectual property of Jennifer Tompkins

Experiment using poorly notated third party widget from Moego
Problem: work around User Data gathered to prevent remembering client log in on one widget locking in to a single location of business.  3 locations (third party only provides landing widget for primary locaiton) but user login remembered from previoius location when embed in squarespace preventing viewing distict widgets depending on locations. No distinct widgets available for each location.
Secondary problem: Impossible to set to open in new tab to work around user data while staying within single origin policy

Primary Solution:
edited widget source code to reflect distinct location links, attempted to add target: _blank but cannot due to SOP, additionally, no access to source code the website the widget refers to so cannot use id specific hyperlinks

Seconday Solution:
provide 3 distict book now links directing to 3 distinct URLs and using target:_blank to prevent saved log in overriding location
additionally made landing page for each location providing essential info while still using embed widget, source code edited to jump to the correllating location. User cannot accidentally navigate past home page and be unable to return, if user desires more info then they can open landing pages and still immediately book or view info then book via location specific widget

INCOMPLETE CONFLICTS (tertiary)
When following direct booking links, problem was successfully resolved in using target_blank to force new tab, however cookies are retained. If user opens multiple tabs, (ie one for each location), location of all tabs will force refresh to location of most recently clicked link. If all tabs are closed, then links still work as expected.

Cannot successfully round edges of widget with border within container. suspect need version of bootstrap that is not 6 years old >.<
Chose to instead visually offset via shadowbox, though unsure why bootstrap shadowbox worked when round border did not. 
