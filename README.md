# javascript30
This is a repository that follows Javascript30 by @wesbos 
https://javascript30.com/ 
### Day 37: October 12, 2017    

**Today's Progress**:   
1. Today I continued with JavaScript30.  

**Thoughts**:     
1. Follow along links.  
2. How to get the element coordinates.  
3. Build an object and read its properties.  
4. CSS property: transform.  
 ```javascript
    const linkCoords = this.getBoundingClientRect()
        const coords = {
        width: linkCoords.width,
        height: linkCoords.height,
        top: linkCoords.top + window.scrollY,
        left: linkCoords.left + window.scrollX
      };
      highlight.style.height = `${coords.height}px`;
      highlight.style.width = `${coords.width}px`;
      highlight.style.transform = `translate(${coords.left}px,${coords.top}px)`
    }
    triggers.forEach(a => a.addEventListener('mouseenter', highlightLink))
  
```
### Day 36: October 11, 2017    

**Today's Progress**:   
1. Today I continued with JavaScript30.  

**Thoughts**:     
1. Device Orientation and Navigator Geolocation.  
 ```javascript
      navigator.geolocation.watchPosition((data) => {
      console.log(data);
    }, (err) => {
      console.error(err);
      alert('HEY! YOU GOTTA ALLOW THAT TO HAPPEN!!!');
    });

    if (window.DeviceOrientationEvent) {
      window.addEventListener('deviceorientation', deviceOrientationHandler, false);
    }
```
### Day 35: October 10, 2017    

**Today's Progress**:   
1. Today I continued with JavaScript30.  

**Thoughts**:     
1. Speech recognition.  
 ```javascript
  window.SpeechRecognition = window.SpeechRecognition || window.webkitSpeechRecognition;
    const recognition = new SpeechRecognition();
    recognition.interimResults = true;
```

### Day 34: October 9, 2017    

**Today's Progress**:   
1. Today I continued with JavaScript30.  

**Thoughts**:     
1. Video
 ```javascript
function getVideo() {
  navigator.mediaDevices.getUserMedia({ video: true, audio: false })
    .then(localMediaStream => {
      console.log(localMediaStream);
      video.src = window.URL.createObjectURL(localMediaStream);
      video.play();
    })
    .catch(err => {
      console.error(`OH NO!!!`, err);
    });
}
```

### Day 33: October 8, 2017    

**Today's Progress**:   
1. Today I continued with JavaScript30.  

**Thoughts**:     
1. 
### Day 32: October 7, 2017    

**Today's Progress**:   
1. Today I continued with JavaScript30.  

**Thoughts**:     
1. Use `e.offsetY` and `e.offsetY` to get the position where he cursor is.
2. `String.prototype.trim()` returns a  new string representing the calling string stripped of whitespace from both ends.
### Day 31: October 5, 2017    

**Today's Progress**:   
1. Today I continued with JavaScript30.  

**Thoughts**:     
1. Today I made toggleAll on Local Tapas 
### Day 30: October 4, 2017    

**Today's Progress**:   
1. Today I continued with JavaScript30.  

**Thoughts**:     
1. Asigning values to strings, numbers or booleans copies will not tu update the orginial value.  
2. Doing it to Array or Objects will. They are not copies, but references.  
3. `e.preventDefault` prevent the page to reload.  
4. `JSON.stringify()`  and `JSON.parse()` Objects to Strings and viceversa.  
5.  Event delegation allows you to avoid adding event listeners to specific nodes;  instead, the event listener is added to one parent.  
6. Using the Element.matches API, we can see if the element matches our desired target.  
### Day 29: October 3, 2017    

**Today's Progress**:   
1. Today I continued with JavaScript30.  

**Thoughts**:     
1. Key Sequence Detection.  
2. Slide In on Scroll.  
### Day 28: October 1, 2017    

**Today's Progress**:   
1. Today I continued with JavaScript30.  

**Thoughts**:     
1. Dev Toll Tricks `console.time`, `console.count`, `console.clear`,`console.group`, `console.dir`, `console, assert`, `console.info`, `console.warn`, `console.error`.  
2. Muiltiple checkboxes. 
3. HTML5 Video Player.  
### Day 27: September 28, 2017    

**Today's Progress**:   
1. Today I continued with JavaScript30.  

**Thoughts**:     
1. Canvas methods
### Day 26: September 27, 2017    

**Today's Progress**:   
1. Today I continued with JavaScript30.  

**Thoughts**:     
1. Array methods `Array.prototype.some()`, ` Array.prototype.every()`, `Array.prototype.find()` , `Array.prototype.findIndex()`.  
### Day 25: September 26, 2017    

**Today's Progress**:   
1. Today I continued with JavaScript30.  

**Thoughts**:     
1. `fetch(endpoint).then(blob=>blob.json()).then(data=> cities.push(...data))` to put the JSON elements into arrays.  
2. `const regex = new RegExp(wordToMatch, 'gi');` to create a Regular expression.  
### Day 24: September 25, 2017    

**Today's Progress**:   
1. Today I continued with JavaScript30.  

**Thoughts**:     
1. toggleOpen will not be excetuted when the document load, toggleOpen() will.  
### Day 23: September 22, 2017    

**Today's Progress**:   
1. Today I continued with JavaScript30.  

**Thoughts**:     
1. Array methods `filter`, `map`, `sort`, `reduce`.  
2. `console.table()`  
### Day 22: September 21, 2017    

**Today's Progress**:   
1. Today I continued with JavaScript30.  

**Thoughts**:     
1. Variables CSS `:root{--name:value}`.  
2. Access to variable `var(--name)`. 
3. Events `change` `mousemove`.
4. HTMLElement.dataset property allows access, both in reading and writing mode, to all the custom data attributes (data-*) set on the element, either in HTML or in the DOM.  
### Day 21: September 20, 2017    

**Today's Progress**:   
1. Today I continued with JavaScript30.  

**Thoughts**:     
1. `transform-origin` by defautl 50%, allows to pivot the element at all.  
2. `transform` allows you to rotate, scale, move, skew, etc., elements.  
3. `transition` allows you to change property values smoothly (from one value to another), over a given duration. `transition-timing-function` https://www.w3schools.com/css/css3_transitions.asp.  



### Day 20: September 19, 2017    

**Today's Progress**:   
1. Today I started with JavaScript30.  

**Thoughts**:     
1. `document.querySelector` returns the first element that matches a specified CSS selector(s) in the document.  
2. `e.propertyName` returns the name of the CSS property associated with the transition, when a transitionevent occurs. This property is read-only.  


