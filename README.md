## Website Performance Optimization portfolio project

## Optimized version of the site is @ http://mandyreal.github.io

General optimizations implemented to achieve required PageSpeed Ingsights score of >90:
- Reduced image file sizes using [TinyJPG](https://tinyjpg.com/)
- Made all style.css as inline
- Used [loadCSS](https://github.com/filamentgroup/loadCSS) to load Google Web fonts asynchronously
- Loaded Google analytics JavaScript asyncronously to avoid render blocking
- Used [Critical Path CSS Selector](http://jonassebastianohlsson.com/criticalpathcssgenerator/) for the bootstrap CSS before making it inline

To achieve the jank-free Pizza site:
- Updated functions changePizzaSizes and updatePositions in main.js to move unnecessary codes outside of for-loops, thereby reducing time spent on those functions
- Reducing the number of sliding pizzas down from 200 to 30
- Used [translate3d](http://davidwalsh.name/translate3d) in the mover class to force hardware acceleration in Webkit

Other references:
- P4 foler in Piazza with all the helpful comments and feedbacks from cohort and instructors
- [Dillinger.io](http://dillinger.io/) was used to edit the README before pushing to github :) 