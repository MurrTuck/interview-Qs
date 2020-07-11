# Interview Study Questions

### HTML/CSS:
* **What is a selector in CSS?**
    * CSS selectors are used to "find" (or select) the HTML elements you want to style. 
    * We can break up the CSS selectors into five categories:
        * Simple selectors (select elements based on name, id, class)
        * Combinator selectors (select elements based on a specific relationship between them)
        * Pseudo-class selectors (select elements based on certain state)
        * Pseudo-elements selectors (select and style a part of an element)
        * Attribute selectors (select elements based on an attribute or attribute value)


#### CSS element Selector Examples 
```
p {
  text-align: center;
  color: red;
}

.center {
  text-align: center;
  color: red;
}

p.center {
  text-align: center;
  color: red;
}

```



### JavaScript:
* **Describe what _context_ is in JavaScript.**
    * Context - Outside of Javascript, context means the surrounding information that gives a better understanding and more clarity to a situation. This also applies the same way to Javascript. 

    * Since objects are the building blocks of Javascript, there is a special object we can use to access the context of our code that is being executed. The object is referred to as ```this```.

    **This**

    The value of ```this``` is decided upon how our code is being executed. 

    **Default Context**
    * The default  value of ```this``` refers to the global object. In a browser environment, ```this``` would be the ```window``` object.

    _Default Context Example_

```
const myCar = 'Tesla'

function displayMyCar() {
  // reference the global object with `this`
  alert(this.myCar)
}

displayMyCar()
```
   **Implicit Context**
* Implicet Context is when the value of ```this``` refers to the object the code is running in. 

    _Impllicit Context Example_

    ```
    const newCar = {
        make: 'Tesla',
        model: 'Model X',
        year: 2019,
        showOff: function(){
            alert(`I drive a ${this.make}`)
        }
    }

    newCar.showOff();
    ```

    **Type of Context**

    _Explicit context_ is when the value of ```this``` is explicitly defined.

    There are three methods that allow us to defind the context of our code:
```
.call()
.apply()
.bind()
```


### React:
* **What is a component in React?**

In React, ```components``` are the building blocks of our apps. 

There are two types of components:
* **Class Components**
* **Functional Components**

Class Components can also be called ```stateful components```.

Functional components can also be called ```stateless components```.

**Class Components**

Class components are built from JavaScript ```classes```, and allow us to store data, called ```state```, in our component. 

_the syntaxt for a class component is as follows:_


    import React, {Component} from 'react';

    class ClassComponent extends Component {
        constructor(){
            super()

            this.state = {
                state: '',
                example: true
            }
        }
        render() {
            return <h1>Hello, I'm a class component</h1>
        }
    }

    export default ClassComponent;


**Functional Components**

Functional Components are build from JavaSCript functions, and are commonly used to compartmentalize functionality. 

Functional components are also often used for static display:


    import React from 'react';

    const FuncComponent = () => {
        return(
            <h1>Hello, I'm a functional component</h1>
        )
    }

    export default FuncComponent;



HTML/CSS: 

What are the different values for the position property in CSS, and how do they work? 
JavaScript: 

Explain some of the differences between let, var, and const.
React: 

What are refs in React?