# jQuery Image Paste Event
jQuery image paste helper class to normalize how to listen for image pasting.  
Pretty straightforward: just include the JS file, and then listen for the `custom/paste/images` event.

### Example
``` javascript
$(document).on({
    'custom/paste/images': function(event, blobs) {
        console.log(blobs);
    }
});
```

### Notes
- Currently will only fire the `custom/paste/images` if there is at least one image detected as available
- Does not currently work in Safari; will update it when I figure it out, or else when Safari updates to make it possible
