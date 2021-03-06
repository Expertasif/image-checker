# NCC Image Checker - Chrome Extension

[![Build Status](https://travis-ci.org/nccgroup/image-checker.svg?branch=development)](https://travis-ci.org/nccgroup/image-checker)

Provides image optimisation information within the browser. 
The quality of layout for the information presented is strongly linked to markdown building techniques used.

## Install
[Download from the Chrome Extension Store](https://chrome.google.com/webstore/detail/fphiheficgnpphmjdliclanppccfgifl)
or
1. Clone the repo
2. Open [Chrome Extensions](chrome://extensions)
3. On the top right, check the checkbox for 'Developer mode'
3. Click 'Load unpacked extension...'
3. Select the directory where you have cloned this repo

## Current limitations
1. overlay of background images where the element is positioned with negative values or via tranform will display as if the values were positive; why? the javascript api returns absolute values
2. overlay of carousel images will display for covered images as well
3. overlapping overlays hide each other
4. file size for some cross origin images is not available (depends of support of performanceEntry)
5. sprites are not bad practice ... yet this tool flags them red, we don't handle them at all
