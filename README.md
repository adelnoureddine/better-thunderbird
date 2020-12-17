# Better thunderbird settings and themes

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
- In config, set ```mailnews.default_sort_order``` to ```2``` and ```mailnews.default_sort_type``` to ```18``` (sort dates descending, so newer emails first)
