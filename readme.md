# APIFRAME Outpaint Mask Tool

This tool allows users to create outpaint masks for images using a lasso selection tool. It's designed to work with the APIFRAME system for image manipulation and generation.

## Features

- Load images from URL
- Interactive lasso selection tool
- Real-time mask generation
- Copy mask data to clipboard
- Reset mask functionality

## How to Use

1. Open the `index.html` file in a web browser.
2. Enter the URL of the image you want to create a mask for in the input field.
3. Use the lasso tool to draw around the area you want to mask:
   - Click to start drawing
   - Continue clicking to add points to your selection
   - Click near the starting point to close the selection
4. The mask data will automatically appear in the text area below the image.
5. Click "Copy Mask" to copy the mask data to your clipboard.
6. Click "Reset Mask" to clear the current selection and start over.

## Technical Details

- The tool uses HTML5 Canvas for drawing the lasso selection.
- Mask generation is done in real-time as you draw.
- The mask is created as a black and white image, where the selected area is white and the rest is black.
- The mask is output as a base64-encoded data URL.

## Files

- `index.html`: The main HTML file containing the user interface.
- `lasso-canvas-image.js`: JavaScript file containing the lasso tool implementation.

## Dependencies

- [Tailwind CSS](https://tailwindcss.com/) (loaded via CDN) for styling.

## Browser Compatibility

This tool should work in all modern browsers that support HTML5 Canvas and ES6 JavaScript features.

## Note

This tool is designed to work with the APIFRAME system. The generated mask data is intended to be used with APIFRAME's image processing capabilities.
