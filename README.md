# Better thunderbird settings and themes

Tested on Thunderbird 78.

## Theme
- In config, set ```toolkit.legacyUserProfileCustomizations.stylesheets``` to ```true```
- Create chrome/ folder in profile folder, then create userChrome.css with :
```
/* Set height for cells in folder pane */
#folderTree > treechildren::-moz-tree-row {
	margin-top: 0px !important;
	height: 25px !important;
}

/* Set height for cells in thread pane */
#threadTree > treechildren::-moz-tree-row {
	border: none !important;
	height: 40px !important;
}
```

## Sorting
- In config, set ```mailnews.default_sort_order``` to ```2``` and ```mailnews.default_sort_type``` to ```18``` (sort dates descending, so newer emails first), or ```mailnews.default_sort_type``` to ```22``` (to sort dates descending and sort by thread)
- Also, set ```mailnews.default_view_flags``` to ```1``` to turn threaded on

More info on sorting [from here](https://superuser.com/questions/13518/change-the-default-sorting-order-in-thunderbird).
