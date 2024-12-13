# Cameron's Custom userChrome for Firefox
This is a collection of random `userChrome.css` mods which I have created to my liking for Firefox.

These are all based on my preferences, but some files have basic editable properties.
I have no idea if editing these properties will break anything, I have written these for my own use, and made them available for others who may be interested in hacking around with them.

# Using these Mods
## Expected Firefox Setup
These mods are intended to be used on Firefox, with the new Sidebar, and Vertical Tabs enabled (some mods may work regardless, some may look odd, others may not work at all).

To enable the new Sidebar and Vertical Tabs, please visit [about:config](about:config) in Firefox, and enable `sidebar.revamp` and `sidebar.verticalTabs`.

Additionally, the Sidebar is intended to be set to *collapsed* by Firefox for the Sidebar mods.

## Installing the userChrome.css
To allow selectively enabling and disabling different mods, along with combining with other userChrome.css you may have, I have left each mod as a separate .css file.

I recommend cloning this repository into the `chrome` directory your Firefox user directory (accessible from [about:profiles](about:profiles))

Once this is done, you can modify your userChrome.css and include `@import` statements for as many or as few mods as you wish. An example (for all current mods) could be:
```css
@import url(firefox-userchrome/sidebar-hover-reveal.css);
@import url(firefox-userchrome/sidebar-remove-bottom-buttons.css);
@import url(firefox-userchrome/sidebar-remove-browser-outline.css);
@import url(firefox-userchrome/url-searchbar-rounded.css);
@import url(firefox-userchrome/url-searchbar-translucent.css);
@import url(firefox-userchrome/custom-browser-pane-margin-and-rounding.css);
```