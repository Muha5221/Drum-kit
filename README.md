# Drum Kit 🥁

A web-based interactive drum kit that responds to both mouse clicks and keyboard presses.

## Features

- Play different drum sounds by clicking buttons or pressing keys
- Visual feedback when a drum is activated
- Responsive design
- Realistic drum sounds

## How to Play

### Using Mouse:
1. Click on any of the drum buttons to play the corresponding sound

### Using Keyboard:
Press these keys to play sounds:
- **w**: Tom 1
- **a**: Tom 2
- **s**: Tom 3
- **d**: Tom 4
- **j**: Crash cymbal
- **k**: Kick bass
- **l**: Snare drum


## Technologies Used

- HTML5
- CSS3
- JavaScript (DOM manipulation, event listeners)
- Web Audio API

## Code Overview

The project works by:

1. Adding click event listeners to all drum buttons
2. Adding keyboard event listeners to the document
3. Playing the appropriate sound based on which button was clicked or key was pressed
4. Providing visual feedback with a button animation

Key functions:
- `handleClick()`: Processes mouse clicks on drum buttons
- `makeSound()`: Plays the appropriate sound based on input
- `buttonAnimation()`: Adds/removes visual feedback

## Customization

You can easily customize this project by:

1. Replacing sound files in the `sounds` directory (keep same filenames)
2. Modifying the styling in `styles.css`
3. Changing the key mappings in `index.js`

## Known Issues

- The default case in the switch statement logs `buttonInnerHTML` which is undefined for keyboard events (should log `key` instead)
- The setTimeout duration in `buttonAnimation` is missing the time parameter (currently just `100` without `ms`)

## Credits

- Drum sounds from various sources
- Inspired by various online drum kit projects

## License

This project is open-source and available for anyone to use or modify.
