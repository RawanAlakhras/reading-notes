# Transforms

* The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.
* The actual syntax for the transform property is quite simple, including the transform property followed by the value. 
  
### 2D Transforms:

* Elements may be distorted, or transformed, on both a two-dimensional plane or a three-dimensional plane. 
* Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. 
* Three-dimensional transforms work on both the x and y axes, as well as the z axis. 
* The transform property accepts a handful of different values:
    1. The rotate value
    2. 2D Scale
    3. 2D Translate
    4. 2D Skew

# Transitions & Animations

* One evolution with CSS3 was the ability to write behaviors for transitions and animations. 
* Animations within CSS3 allow the appearance and behavior of an element to be altered in multiple keyframes.
* Transitions provide a change from one state to another, while animations can set multiple points of transition upon different keyframes.

### Transitions

* There are four transition related properties in total:
    1. transition-property
    2. transition-duration
    3. transition-timing-function
    4. transition-delay

# 8 SIMPLE CSS3 TRANSITIONS

* Fade in :Fade in effects are coded in two steps: first, you set the initial state; next, you set the change,
*  Change color: Animating a change of color used to be unbelievably complex, with all kinds of math involved in calculating separate RGB values and then recombining them
* Grow & Shrink: To grow an element, you used to have to use its width and height, or its padding. But now we can use CSS3’s transform to enlarge.
* Rotate elements: CSS transforms have a number of different uses, and one of the best is transforming the rotation of an element
* Square to circle: With CSS, it’s a simple effect to achieve, we just transition the border-radius property.
* 3D shadow:3D shadows were frowned upon for a year or so, because they weren’t seen as compatible with flat design, which is of course nonsense, they work fantastically well to give a user feedback on their interactions and work with flat, or fake 3D interfaces.
* Swing
* Inset border:One of the hottest button styles right now is the ghost button; a button with no background and a heavy border. We can of course add a border to an element simply, but that will change the element’s position. We could fix that problem using box sizing, but a far simpler solution is the transition in a border using an inset box shadow.
