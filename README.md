#koGrid : A Knockout DataGrid#

__Contributors:__

KoGrid Team:
* [Eric M. Barnard](https://github.com/ericmbarnard/koGrid) 
* [Tim Sweet](http://ornerydevelopment.blogspot.com/)
* [Jonathon Ricaurte](https://github.com/xcrico)

License: [MIT](http://www.opensource.org/licenses/mit-license.php)

Dependencies: jQuery & Knockout
***
##About##
__koGrid__ is a direct knockout port of [ng-grid](http://angular-ui.github.com/ng-grid/) which was originally inspired by koGrid, which was inspired by SlickGrid. I know, right?

koGrid is in 2.0.3 release currently. 

***
_The sizzle_:

```html
<div data-bind="koGrid: { data: myObservableArray }"></div>
```
```javascript
var vm = {
  myObservableArray: ko.observableArray(/* array of any complex obects */)
};

ko.applyBindings(vm);
```

##Want More?##
Check out the [Getting Started](https://github.com/ericmbarnard/KoGrid/wiki/Getting-Started) and other [Docs](https://github.com/ericmbarnard/KoGrid/wiki)

##2.0 Examples##
#Coming Soon...#

##1.2 Examples##
* [Simple Example](http://ericmbarnard.github.com/KoGrid/examples/SimpleExample.html) : Shows the absolute bare-minimum needed to get up and running
* [Defined Columns Example](http://ericmbarnard.github.com/KoGrid/examples/DefinedColumns.html) : Shows a grid with columns defined
* [Complex Example with Server Side Paging, Filtering, Sorting](http://ericmbarnard.github.com/KoGrid/examples/Complex-Server-Side-Paging.html) : Shows an example that easily allows server-side paging, sorting, and filtering
* [Large Data Set](http://ericmbarnard.github.com/KoGrid/examples/LargeData.html) : 10000+ rows! Shows virtualized scrolling, sorting and filtering
* [Master-Details](http://ericmbarnard.github.com/KoGrid/examples/MasterDetails.html) : Shows an example of Master-Detail display (click on row to display details)

also check out the new [Custom Cell Template Library](https://github.com/ericmbarnard/KoGrid/wiki/Cell-Template-Library)
##Change Log##
* __2012-12-13__ - Version 2.0 BREAKING CHANGES. numerous enhancements, bugfixes and architectural changes. reduced code footprint by ~40%.
* __2012-08-30__ - Version 1.2 merging changes from skoGrid branch
* __2012-08-18__ - Adding new features, up/down arrows now control the selected item when multiselect is disabled. columnDefs are now observable so you can change the columns on the fly.
* __2012-08-16__ - Styles moved into CSS, minor bug fix for Row templates where cells wouldn't take null values (for instance, when you want to display an image instead of the value)
* __2012-03-07__ - Huge Row Rendering Perf improvements, Easier syntax for custom cell templates,  Allow Custom CSS Classes on Header and Data Cells, Allow toggling of Footer Visibility, Much better button iconography, enhanced default CSS styles, various other bug fixes
* __2012-04-10__ - Wildcard Filtering, better grid resizing during window resize events, better sorting, numerous bug-fixes