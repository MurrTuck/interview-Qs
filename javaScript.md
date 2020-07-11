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