## General Information
* [Alloy Documentation](http://docs.appcelerator.com/titanium/3.0/#!/guide/Alloy_Framework)
* [Alloy on NPM](https://npmjs.org/package/alloy)

## Coming Features
The following are planned features for the next release:
* [ALOY-394](http://jira.appcelerator.org/browse/ALOY-394). Model-view binding on Views using collections, allowing for arbitrary component repetition.
* [ALOY-387](https://jira.appcelerator.org/browse/ALOY-387). [ALOY-388](https://jira.appcelerator.org/browse/ALOY-388). View (XML) and controller (JS) code completion in Titanium Studio.
* [ALOY-382](https://jira.appcelerator.org/browse/ALOY-382). [ALOY-383](https://jira.appcelerator.org/browse/ALOY-383). Support in markup for attributes like rightNavButton, leftNavButton, and searchbar
* [ALOY-103](https://jira.appcelerator.org/browse/ALOY-103). Model-view binding of models to discrete properties on UI components.

## 0.3.3 (30 November 2012)

### New features
* [ALOY-104](http://jira.appcelerator.org/browse/ALOY-104). Enable Model-View binding on TableViews. For more information, see the [todo_binding test application](https://github.com/appcelerator/alloy/tree/master/test/apps/models/todo_binding).
* [ALOY-312](http://jira.appcelerator.org/browse/ALOY-312). Update Underscore.js to version 1.4.2 and Backbone.js to minified production 0.9.2 version.
* [ALOY-373](http://jira.appcelerator.org/browse/ALOY-373). [ALOY-379](http://jira.appcelerator.org/browse/ALOY-379). Add Collection tag in markup to create a singleton or instance(s) of a collection.
* [ALOY-390](http://jira.appcelerator.org/browse/ALOY-390). [ALOY-391](http://jira.appcelerator.org/browse/ALOY-391). Add Model tag in markup to create a singleton or instance(s) of a model.
* [ALOY-396](http://jira.appcelerator.org/browse/ALOY-396). [ALOY-397](http://jira.appcelerator.org/browse/ALOY-397). [ALOY-156](http://jira.appcelerator.org/browse/ALOY-156). Add completion callback to all methods in the animation.js builtin library.
* [ALOY-403](http://jira.appcelerator.org/browse/ALOY-403). Add Alloy.Collection.instance() and Alloy.Models.instance() methods to create an instance of a collection or model, respectively.
* [ALOY-367](http://jira.appcelerator.org/browse/ALOY-367). [ALOY-377](http://jira.appcelerator.org/browse/ALOY-377). Alloy apps now work with Soasta touch test.

### Bugs fixes and improvements
* [ALOY-311](http://jira.appcelerator.org/browse/ALOY-311). Improve Ti.UI.Android.MenuItem parser.
* [ALOY-370](http://jira.appcelerator.org/browse/ALOY-370). Fix ability to assign functions with variable assigned functions in controllers.
* [ALOY-376](http://jira.appcelerator.org/browse/ALOY-376). Improve handling of Ti.Android.Menu component.
* [ALOY-393](http://jira.appcelerator.org/browse/ALOY-393). (Re-)enable optimizer.js as part of runtime JavaScript file optimization.
* [ALOY-401](http://jira.appcelerator.org/browse/ALOY-401). Change Alloy.globals namespace to Alloy.Globals.

## 0.3.2 (15 November 2012)

### Bug fixes and improvements
* [ALOY-353](http://jira.appcelerator.org/browse/ALOY-353). Support all Backbone eventing in Titanium proxies, on(), off(), trigger(). Fixed multiple event firing bug with on().
* [ALOY-355](http://jira.appcelerator.org/browse/ALOY-355). Improve path handling in compiler plugin for OS X.
* [ALOY-356](http://jira.appcelerator.org/browse/ALOY-356). Remove string builtin dependency to shorten compilation time.
* [ALOY-365](http://jira.appcelerator.org/browse/ALOY-365). Add Alloy.globals namespace for global context.
* [ALOY-380](http://jira.appcelerator.org/browse/ALOY-380). Create app/alloy.js file automatically for all new projects.

## 0.3.1 (2 November 2012)

### New features
* [ALOY-192](http://jira.appcelerator.org/browse/ALOY-192). Add to-do sample application. Code is available on [github](https://github.com/appcelerator/alloy/tree/master/test/apps/models/todo).
* [ALOY-337](http://jira.appcelerator.org/browse/ALOY-337). Support themes to change the appearance of the entire GUI by customizing styles and assets. For more information, see:
    * [Alloy Styles and Themes](http://docs.appcelerator.com/titanium/3.0/#!/guide/Alloy_Styles_and_Themes)
    * [Themes sample application on github](https://github.com/appcelerator/alloy/tree/master/test/apps/advanced/themes)

### Bug fixes and improvements
* [ALOY-306](http://jira.appcelerator.org/browse/ALOY-306). Support platform, formFactor, and inline event attributes with abstract types in markup.
* [ALOY-340](http://jira.appcelerator.org/browse/ALOY-340). Fix Android "too deep recursion while parsing" error with Rhino runtime.
* [ALOY-341](http://jira.appcelerator.org/browse/ALOY-341). Improve adapter-backbone processing.
* [ALOY-352](http://jira.appcelerator.org/browse/ALOY-352). Fix SQL adapter to work if no migrations are present.
* [ALOY-354](http://jira.appcelerator.org/browse/ALOY-354). Fix "alloy generate jmk" command.

0.3.0 (beta)
------------
* Removed node-appc dependency.
* Added Alloy splash screens and icons
* Updated widgets, added new button-grid widget.
 
0.2.42
--------
* Ti.UI.OptionDialog markup parser added. Check out this link for a test app and usage: [https://github.com/appcelerator/alloy/tree/master/test/apps/ui/optiondialog](https://github.com/appcelerator/alloy/tree/master/test/apps/ui/optiondialog)
* You can get the Alloy version at runtime now with `Alloy.version`
* Tightened up XML ID restrictions. As an enforced best practice, no reserved JS words as IDs. If you try to, you'll get a compile time error message.
* Revamp of code processing, better organized, more efficient. It's all under the hood, you shouldn't notice, other than compiles might be faster.
* Quick fix to error output in compiler plugin.py
* Some minor cleanup in the test apps
