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
