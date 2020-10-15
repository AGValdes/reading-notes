# Class 14 Reading Notes

 ## What Google Learned About building Teams

 Google did a lot of research into what makes a good team. The best teams in this study shared 2 qualities:
 - Everyone in the group was allowed to speak and contribute an equal amount.
 - People on the team had a high average social sensitivty, meaning they pick up on social queues well and are good at picking up on how others are feeling.
## Transforms
- CSS3 transforms are not supported on all browsers, but add dynamic effects to your page.
### 2D Transforms:
- Rotate
- Scale
- Translate
- Skew
The **default transform origin** the **center of the element**
### 3D Transforms:
- In order for three-dimensional transforms to work the elements need a **perspective** from which to transform. 
- As with setting a transform-origin you can also set a perspective-origin.
- Rotate
- Translate
- Skew
## Transitions and Animations
### Transitions
- With CSS3 transitions you have the potential to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.
- There are four transition related properties in total, including **transition-property**, **transition-duration**, **transition-timing-function**, and **transition-delay**.
- It is important to note, not all properties may be transitioned, only properties that have an identifiable halfway point.
- The duration in which a transition takes place is set using the transition-duration property. The value of this property can be set using general timing values, including seconds (s) and milliseconds (ms)
- The transition-timing-function property is used to set the speed in which a transition will move.
- The delay sets a time value, seconds or milliseconds, that determines how long a transition should be stalled before executing. 
### Animations
- To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.
- Once the keyframes for an animation have been declared they need to be assigned to an element. To do so, the animation-name property is used with the animation name, identified from the @keyframes rule, as the property value
- Once you have declared the animation-name property on an element, animations behave similarly to transitions. They include a duration, timing function, and delay if desired.
- By default, animations run their cycle once from beginning to end and then stop.
- To have an animation repeat itself numerous times the animation-iteration-count property may be used.
- Values for the animation-iteration-count property include either an integer or the infinite keyword. 
- Using an integer will repeat the animation as many times as specified, while the infinite keyword will repeat the animation indefinitely in a never ending fashion.
 ## Cool CSS Transitions

 - **Fade In** Fade in effects are coded in two steps: first, you set the initial state; next, you set the change, for example on hover:
 - `.fade
{
        opacity:0.5;
}
.fade:hover
{
        opacity:1;
}`
- **Color changing** set the div’s class to “color” and specify the color we want in our CSS: 
- `.color:hover
{
        background:#53a7ea;
}`
- **Grow and Shrink** use CSS3’s transform to enlarge
- `.grow:hover
{
        -webkit-transform: scale(1.3);
        -ms-transform: scale(1.3);
        transform: scale(1.3);
}`
- **Rotate Elements** CSS transforms have a number of different uses, and one of the best is transforming the rotation of an element
- `.rotate:hover
{
        -webkit-transform: rotateZ(-30deg);
        -ms-transform: rotateZ(-30deg);
        transform: rotateZ(-30deg);
}`
- **Square to Circle**  just transition the border-radius property.
- `.circle:hover
{
        border-radius:50%;
}'
- **3D Shadow**This effect is achieved by adding a box shadow, and then moving the element on the x axis using the transform and translate properties so that it appears to grow out of the screen.
- `.threed:hover
{
        box-shadow:
                1px 1px #53a7ea,
                2px 2px #53a7ea,
                3px 3px #53a7ea;
        -webkit-transform: translateX(-3px);
        transform: translateX(-3px);
}`
- **Swing** Not all elements use the transition property. We can also create highly complex animations using @keyframes, animation and animation-iteration. due to implementation issues, we need to use @-webkit-keyframes as well as @keyframes
- `.swing:hover
{
        -webkit-animation: swing 1s ease;
        animation: swing 1s ease;
        -webkit-animation-iteration-count: 1;
        animation-iteration-count: 1;
}`
- **Inset Border** 
- `.border:hover
{
        box-shadow: inset 0 0 0 25px #53a7ea;
}`

[Back to Top](#) [Back to Code 201](code201notes.md) [<-- Back](README.md)