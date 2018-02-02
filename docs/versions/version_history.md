---
id: version_history
title: Version History
layout: hero
sectionid: versions
permalink: versions/version_history.html
redirect_from:
  - "versions/index.html"
---

## ReactXP Versioning

### Versioning Strategy
A new version of ReactXP will be released a monthly basis (approximately), following the same general update timeline of React Native. Each new version will get its own branch, allowing consumers of the library to take a dependency on a stable code base.


### Version History

#### Version 0.51.4 of reactxp
_Released 2 Feb 2018_

Fixed regression in RootView getStateFromStore() method

#### Version 0.51.3 of reactxp
_Released 31 Jan 2018_

#### Version 0.51.2 of reactxp
_Released 25 Jan 2018_

Prevent web page reload when hitting enter in RX.TextInput.
Fix announcement issue on Android devices.

#### Version 0.51.1 of reactxp
_Released 20 Jan 2018_

Fixed regression in Animated.View blur() method

#### Version 0.51.0 of reactxp
_Released 18 Jan 2018_

Fixed focusable View condition for VoiceOver in web implementation.
Exposed web-specific ariaRoleDescription prop to work around other VoiceOver issues.
Updated RN for Windows UWP dependency.
Fixed recent regression that broke focus and blur calls in iOS and Android implementations of AnimatedTextInput.

#### Version 0.51.0-alpha.9 of reactxp
_Released 17 Jan 2018_

Removed console error related to animations of values not currently associated with any mounted component. It was too noisy.

#### Version 0.51.0-alpha.8 of reactxp
_Released 16 Jan 2018_

Fixed bug in Windows UWP implementation related to selection ranges in TextInput.
Fixed screen reader issue in Mac implementation.
Removed ```textAlign``` prop from TextInput. It was extraneous, since it's already supported as a style attribute.
Updated Windows UWP dependency to use the latest version of RN for UWP.
Worked around issue with screen readers on Chrome browsers.
Added currentTarget field back to SyntheticEvent.
Added support for "switch" aria type (web implementation).
Fixed recent regression in web animation code.

#### Version 0.51.0-alpha.5 of reactxp
_Released 11 Jan 2018_

Eliminated limitation within RX.Button where only one child element was allowed.
Fixed regression where native implementation of RX.View with onPress handler didn't provide touch feedback.

#### Version 0.51.0-alpha.4 of reactxp
_Released 10 Jan 2018_

Added code to native implementation of RX.Network so it works with versions of RN before and after 0.48.x.
Fixed regression in web implementation of RX.TextInput.
Fixed bug that caused incorrect behavior of RX.Modal on native platforms.

#### Version 0.51.0-alpha.2 of reactxp
_Released 9 Jan 2018_

Fixed bug in native implementation of RX.ActivityIndicator. It wasn't properly handling the delay prop.
Added support in web implementation of RX.TextInput for custom keyboard types on mobile web browsers.
Added focus and keyboard navigation support for native UWP platform.
Added support for injection of HTML content into RX.WebView.
Added support for postMessage and onMessage handler in RX.WebView for bidirectional communication.

#### Version 0.51.0-alpha.1 of reactxp
_Released 6 Jan 2018_

Fixed break in device dimension change event due to change in RN.
Removed use of RX.Button implementation within RX.View for native-common implementation.
Fixed bug in web implementation of RX.Clipboard.getText. It shouldn't throw.
Fixed timing bug in web implementation of GestureView.
Fixed popup positioning for right-to-left languages in native-common implementation.
Fixed bug in web implementation of TextInput that caused assertion in React.
Breaking change: Removed 'cursor' prop from RX.Button. It was redundant with the 'cursor' style.
New feature: RX.Input.key[Up|Down]Event now allow event subscribers to cancel the event.
New feature: Changed RX.Modal.isDisplayed to accept undefined parameter, in which case it determines whether _any_ modal is displayed.
New feature: Added RX.Popup.isDisplayed method.
Reimplemented web implementation of animation APIs. Removed many limitations of previous implementation and fixed several bugs. Documented remaining limitations.
Fixed bug in web implementation of RX.TextInput that resulted in assertions within React.
Fixed bug in web implementation of RX.Picker. It wasn't correctly combining styles.
Added support in web implementation of RX.TextInput for keyboard type (applicable on mobile web browsers).
Removed use of deprecated RX.NetInfo.fetch method.

#### Version 0.46.6 of reactxp
_Released 13 Dec 2017_

Fixed potential crash in web implementation of RX.ScrollView.
Fixed bug in UWP implementation of RX.Popup, allowing background to be clickable.
In web implementation of RX.ScrollView, added support for clicking on scroll bar to adjust position of thumb.
Added dev warning when using nested RX.Button items.
Fixed a potential crash in web implementation of RX.GestureView.
Implemented drag-and-drop support in UWP implementation of RX.View.

#### Version 0.46.5 of reactxp
_Released 31 Oct 2017_

Added Android "mode" prop to Picker.
Added type definitions for RX.Stateless and RX.ComponentBase.
Updated to React 16.0.0 and React-Dom 16.0.0.
Added RX.UserInterface.registerRootView API to allow registration of secondary views. Also added rootViewId option to RX.Modal and RX.Popup so they can be displayed on secondary views.
Fixed bug in focus restoration on web implementation.
Replaced use of deprecated BackAndroid with BackHandler, avoiding deprecation warnings.
Fixed bug in RX.Button RN implementation where opacity was not property restored after changing disabled prop.

#### Version 0.46.3 of reactxp
_Released 7 Oct 2017_

Added missing focus() method to RX.Animated.View interface.
Exported RX.AnimatedImage, RX.AnimatedText, RX.AnimatedTextInput, and RX.AnimatedView.
Added accessibilityLiveRegion prop to ViewProps for Android and web.
Exported explicit types for ShadowOffset, ScrollIndicatorInsets.
Fixed crash in web RootView when clicking on a popup anchor.
Fixed race condition in hover of Button on web.

#### Version 0.2.2 of reactxp-video
#### Version 1.0.13 of reactxp-navigator
#### Version 0.2.7 of reactxp-imagesvg
#### Version 0.1.6 of reactxp-virtuallistview
_Released 21 Sep 2017_

Updated for RN 0.46 compatibility.
Removed custom react.d.ts and react-dom.d.ts files in favor of public versions.

#### Version 0.46.2 of reactxp
_Released 21 Sep 2017_

Added onContextMenu support on web for Text components.
Exposed attributes to make menus and listboxes accessible on web.
Added new RX.Animated.createValue and RX.Animated.interpolate methods. The old way of instantiating a value and creating an interpolation will be deprecated going forward.
Made a breaking change to Alert.show interface - combined optional parameters into an AlertOptions interface. This will allow for better extensibility in the future.
Updated RN dependency to 0.46.
Removed custom react.d.ts and react-dom.d.ts files in favor of public versions.

#### Version 0.46.0_rc.2 of reactxp
_Released 19 Sep 2017_

Changed RX.Link props to make url mandatory.
Added new Alert implementation for web. It now presents a modal-based themable dialog box.
Fixed bug in ScrollView styles from previous release.
Exposed aria-checked property on button type for web.
Added key attribute to KeyboardEvent.
Fixed bug in web code where onScrollBeginDrag and onScrollEndDrag were called unconditionally even if they were undefined.
Enabled strict null checks in TS compiler and fixed a number of bugs that were exposed.

#### Version 0.46.0_rc.1 of reactxp
_Released 5 Sep 2017_

First pre-release version of 0.46.
Removed Navigator component and moved to an extension.
Fixed style definition for ScrollView so it doesn't include child-related flexbox styles, which aren't supported.

#### Version 0.42.0 of reactxp
_Released 5 Sep 2017_

Removed rc from version.

#### Version 0.42.0_rc.25 of reactxp
_Released 18 Aug 2017_

On web, if there's a queued onScroll event when the scroll position is manually set, cancel the onScroll.

#### Version 0.42.0_rc.24 of reactxp
_Released 9 Aug 2017_

Added accessibility support for GestureView.
Fixed bug in web version that prevented animated fontSize from working.

#### Version 0.42.0_rc.22 of reactxp
_Released 30 July 2017_

On RN platforms, initialProps is now passed to the main view.
Added new PopupOptions field preventDismissOnPress that prevents the popup from being dismissed implicitly when the user clicks or taps outside of the popup or the anchor.
Fixed bug in web implementation of TextInput where border styling was not honored.
Fixed bug on Android that allowed presses to background of Modal to go through.

#### Version 0.42.0_rc.20 of reactxp
_Released 15 July 2017_

Updated to TypeScript 2.4, which caught several bugs in the ReactXP code.
Made Styles.combine much more flexible - it now supports arbitrarily nested arrays of styles.
Changed Network API namespace for detecting network type so it's consistent with other ReactXP APIs. Added documentation.

#### Version 0.1.6 of reactxp-video
_Released 15 July 2017_

Updated to TypeScript 2.4 and made changes to work with latest ReactXP core.

#### Version 0.2.4 of reactxp-imagesvg
_Released 15 July 2017_

Updated to TypeScript 2.4 and made changes to work with latest ReactXP core.

#### Version 0.42.0_rc.18 of reactxp
_Released 13 July 2017_

Fixed runtime crash when running web implementation in Electron.
Added a way to provide screen reader focus to TextInput on web.

#### Version 0.42.0_rc.17 of reactxp
_Released 4 July 2017_

Added ability to set accessibility focus for text input controls.
Added support for iOS-specific ActivationState for RN extensions.

#### Version 0.42.0_rc.16 of reactxp
_Released 30 June 2017_

Fixed another bug in handling of default border width on web.
Added setFocusRestricted and setFocusLimited methods and support for nested keyboard focus on web.
Added isNavigatingWithKdyboard method and keyboardNavigationEvent.


#### Version 0.42.0_rc.12 of reactxp
_Released 16 June 2017_

Added support for new limitFocusWidth prop for constraining keyboard focus.
Fixed bug in handling of mailto URLs on web in the Link component.
Added support for flexGrow, flexShrink, and flexBasis props.


#### Version 0.42.0_rc.11 of reactxp
_Released 13 June 2017_

Fixed bugs in web implementation of focus manager.
Added new API (enableTouchLatencyEvents) and event (touchLatencyEvent) in UserInterface namespace for detecting delays in touch event handling.
Fixed crash in native implementation of Link component that resulted in uncaught exception for some types of links.
Fixed flexDirection style default for web implementation in Image component.
Fixed inconsistency in handling of borders between web and RN when borderStyle is not specified.


#### Version 0.42.0_rc.10 of reactxp
_Released 25 May 2017_

Added new International API namespace for controlling right-to-left mirroring behavior.


#### Version 0.1.2 of reactxp-virtualistview
_Released 23 May 2017_

Republished because index files were missing in previous publish.


#### Version 0.42.0_rc.9 of reactxp
_Released 17 May 2017_

Fixed bug in Navigator that caused crash in hello-world sample.


#### Version 0.42.0_rc.8 of reactxp
_Released 16 May 2017_

Removed Profiling API namespace and dependency on react-addons-perf.


#### Version 0.1.1 of reactxp-virtualistview
_Released 11 May 2017_

Republished because "dist" directory was missing in previous publish.


#### Version 0.1.2 of reactxp-video
_Released 11 May 2017_

Published first version of reactxp-video extension.


#### Version 0.2.0 of reactxp-imagesvg
_Released 10 May 2017_

Switched from old version of react-native-art-svg to latest version of react-native-svg.


#### Version 0.42.0_rc.5 of reactxp
_Released 10 May 2017_

Fixed incorrect import path (using wrong case).
Fixed bug in native View implementation - was using stale props.
Added importantForLayout prop on View (web specific).
Fixed bug in native NavigatorExperimentalDelegate - was using wrong props.


#### Version 0.42.0_rc.4 of reactxp
_Released 27 Apr 2017_

Changed web implementation of Text to prevent copying text to clipboard.
Eliminated the need to specify box-sizing CSS in external CSS file.
Fixed accessibility focus bugs.


#### Version 0.42.0_rc.3 of reactxp
_Released 26 Apr 2017_

Added onLongPress prop for Link.
Fixed accessibility bug relating to Modal dialogs.


#### Version 0.42.0_rc.2 of reactxp
_Released 18 Apr 2017_

Added missing box-sizing CSS directives for web.
Fixed bug in native implementation of View related to accessibility.


#### Version 0.1.0 of reactxp-imagesvg
_Released 26 Apr 2017_

Published first version of reactxp-imagesvg extension.


#### Version 0.42.0_rc.1 of reactxp
_Released 9 Apr 2017_

Updated project to use recent versions of React (15.5.3) and React Native (0.42.3).


#### Version 0.34.3 of reactxp
_Released 7 Apr 2017_

Added new props to ScrollView. Updated package.json to properly reflect peerDependencies on react and react-native.


#### Version 0.34.1 of reactxp
_Released 6 Apr 2017_

This is the initial public release of the ReactXP core library. It is built against React Native 0.34. We are working on updating it to a newer version of React Native, and this will be released shortly.
