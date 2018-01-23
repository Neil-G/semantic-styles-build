## Modifying styles


### The Styling Itself
The styling itself is defined in ```src/definitions/```
variables used in the styling get loaded from 6 different files in this order:

### Site Variables
1. Defaults pulled from ```src/themes/default/globals/site.variables```
2. Packaged theme overrides pulled for site from ```src/themes/{themename}/globals/site.variables```
3. Site overrides pulled from ```src/site/globals/site.variables```

### Component Variables
4. Button default variables from ```src/themes/default/elements/{elementname}.variables```
5. Button packaged-theme variables from ```src/themes/{themename}/elements/{elementname}.variables```
6. Button's site theme from ```src/site/elements/{elementname}.variables```

There are also override files. Read more about that here http://learnsemantic.com/themes/overview.html



## Adding components

Sometimes you want to add entirely new components.  This can done using the following steps:

1. add to name of the file to ```components.js```
2. add the new component to ```/src/theme.config``` similar to the other components
3. add the styling to ```/definitions```



## Important

Keep ```src/theme.config``` and ```components.js``` in sync!  They should contain the same components (uncommented) or else some components won't get recompiled on watch.  Comment out unused components in both of these files to omit them from compilation.



# Background Information on Semantic UI

http://learnsemantic.com/
