# Test Case for Chrome Sidepanel with Materialize CSS - Collapsibles

This is a test case for a Chrome extension that uses the side panel feature with Materialize CSS. The side panel contains a collapsible component that can be expanded and collapsed.

However, the collapsible does not render correctly. As you can see in the screenshot below, the inital height of the list is too small. It does not extend to the bottom of the viewport. It cuts off the collapsibles 6. - 11. Even scrolling is not possible.

![Collapsible not working](collapsible-not-working.png)

Further the nested collapsible items under 2. are not cropped as well. When you close the section 2.1 2.2 appears. See screenshot below.

![Nested Collapsible not working](nested-collapsible-not-working.png)

~~I suspect that the issue is related to the way the side panel (of Chromium) is implemented. When running the HTML in a standard browser window, everything works as expected.~~

 Version: 128.0.6613.115 (Official Build) (arm64)

I created a minimal example to demonstrate the issue. You can find it [here](https://github.com/KajKandler/ce-sidepanel-colapsible-test).

~~If you have any ideas on how to fix this, please let me know.~~

It turns out this is a version issue of materialize css. The old version 1.0.0 has working collapsibles. The current version 2.1.0 doesn't.



Cheers
Kaj