Checkbox - Addon for Phaser by photonstorm
---

This addon give you the option to use checkbox-elements in Phaser.
The function for creating this element, will be automaticly integrated into the Phaser.GameObjectFactory.

Clone from: http://www.phaser-lernen.de/phaser-addons/checkbox/

```Example for using:
/**
 * checkbox function
 * @class
 * @param {number}      _x          horizontal position
 * @param {number}      _y          vertical position
 * @param {object}      _labelObj   object for the textual part of the checkbox contains @param {string} text 
                                    for the label and @param {object} style for the textfield style
 * @param {string}      _sprite     key - The key used to a stored texture in Phase Cache
 * @param {boolean}     _state      predefined state of checkbox (default: false)
 * @return {object}                 A newley created checkbox-object
 */

// creating checkbox
var checkbox1 = game.add.checkbox( 10, 10, { text: 'labeltext', style: { fill: '#ffffff' } }, 'texture' );

// disable checkbox
checkbox1.enabled = false;

// get state form checkbox
alert( checkbox1.state );

// adding click-event
checkbox1.events.onInputUp.add( function( elm, pointer ){
    alert( checkbox1.state );
}, this );```
