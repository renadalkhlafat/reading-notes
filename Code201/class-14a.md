# Transform 
Is a property to position and alter elements.

**Example**

    div {
     -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
      }

**Values for transform**

+ scale
+ translate
+ skew
+ rotate

# Transitions & Animations
### Transitions :
property to alter the appearance and behavior of an element whenever a state change occurs, such as when it is hovered over, focused on, active, or targeted.

    .box {
    background: #2db34a;
    transition-property: background;
    transition-duration: 1s;
    transition-timing-function: linear;
    }


    .box:hover {
    background: #ff7b29;
    }

### Animations:
we use Animations to set multiple points at which an element should undergo a transition

      @keyframes slide {
     0% {
      left: 0;
      top: 0;
      }
    }