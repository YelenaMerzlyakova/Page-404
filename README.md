# Page-404

:no_entry_sign: **WARNING! FLASHING IMAGES!! LOOK AT THE IMAGE FIRST** :no_entry_sign:

This is a second 404-page I created, just for fun. Please be carefull, this page contains flashing images that can cause seizures
if you are prone to them. Otherwise have [fun!](https://yelenamerzlyakova.github.io/Page-404/)

## Objectives

- Improve the semantic HTML
- Know more CSS properties
- Improve your skill in CSS positioning


## Instructions

- Create a repository in Github **404-Page**
- Create your 404 page in **HTML** and **CSS**
- Here's some [inspirations](https://www.google.be/search?q=landing+page&espv=2&source=lnms&tbm=isch&sa=X&sqi=2&ved=0ahUKEwjmvai3v6zTAhVBCSwKHfOIAGMQ_AUIBigB&biw=1250&bih=703#tbm=isch&q=404+page)
- Create a button **back** on the 404 page that redirects to your GitHub profile



## Bonus

- Add animation when we scroll over an element


## Resources

- [CSS3 Animations](https://www.w3schools.com/css/css3_animations.asp)
- [animate.css](https://daneden.github.io/animate.css/)

## Result 

![404](https://github.com/YelenaMerzlyakova/Page-404/blob/master/404.png)

## Glitch Code

The glitch is created by layering different images with different colors that all move at a different speed. 

```
.glitch {
    animation: glitch-skew 8s 8s infinite;
    font-family: tahoma, sans-serif;
    font-size: 8em;
    font-weight: bold;
    line-height: 1;
    position: absolute;
    text-align: center;
    text-transform: uppercase;
    transform-origin: center top;
    display: inline-block;
    color: #030329;
}
  
.glitch__main {
    color: #030329;
}
  
.gc {
    height: 100%;
    opacity: 0.8;
    transform-origin: center center;
    width: 100%;
    z-index: -1;
    position: absolute;
    display: block;
}

.gb {
    height: 100%;
    opacity: 0.8;
    transform-origin: center center;
    width: 100%;
    z-index: -1;
    position: absolute;
    margin-right:  50%;
}
  
.gc-red {
    animation: glitch 300ms  infinite;
    color: red;
}
  
.gc-blue {
    animation: glitch 300ms infinite reverse;
    color: blue;
}
  
.gc-green {
    animation: glitch 300ms 100ms infinite;
    color: green;
}

  
.gb-red {
    animation: glitch 300ms  infinite;
    color: red;
}
  
.gb-blue {
    animation: glitch 300ms infinite reverse;
    color: blue;
}
  
.gb-green {
    animation: glitch 300ms 100ms infinite;
    color: green;
}
  
  
.gl {
    animation: glitch-line 2s linear infinite;
    background: #030329;
    content: '';
    height: 1px;
    position: relative;
    width: 100%;
    z-index: 1;
}

  
  
@keyframes glitch {
    0% {
      transform: translate(0);
    }
    20% {
      transform: translate(-8px, 8px);
    }
    40% {
      transform: translate(-8px, -8px);
    }
    60% {
      transform: translate(8px, 8px);
    }
    80% {
      transform: translate(8px, -8px);
    }
    100% {
      transform: translate(0);
    }
}
  
@keyframes glitch-skew {
    0% {
      transform: skew(0deg, 0deg);
    }
    48% {
      transform: skew(0deg, 0deg);
      filter: blur(0);
    }
    50% {
      transform: skew(-20deg, 0deg);
      filter: blur(4px);
    }
    52% {
      transform: skew(20deg, 0deg);
    }
    54% {
      transform: skew(0deg, 0deg);
      filter: blur(0);
    }
    100% {
      transform: skew(0deg, 0deg);
    }
}
  
@keyframes glitch-line {
    0% {
      top: 0;
    }
    100% {
      top: 100%;
}
}
