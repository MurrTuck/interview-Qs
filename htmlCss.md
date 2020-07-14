
Question found at: 

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

Question found at: https://lms.devmountain.com/courses/70/pages/codewars-kata-string-repeat?module_item_id=21732


HTML/CSS: 

* What are the differences between the caret ( > ), comma ( , ), space (   ), and addition ( + ) selectors in CSS?

  * The caret (>) selector selects nodes that are direct children of the first element.
  * **SYNTAX:**  *A > B*
  * **EXAMPLE:** *ul > li* will match all ``` <li> ``` elements that are nested directy inside the ``` <ul> ``` element. 

  * The comma (,) selector could also combine into a selector list, by adding a comma between them. 
  ```
  h1, .special { 
  color: blue; } 
  ```
  * White space is valid before and after the the comma. You may also find the selectors more readable if each is on a new line. 
  ```
  h1, 
  .special {
  color: blue; 
  } 
  ```

* The addition (+) selector is an Adjacent sibling combinator. The (+) combinator selects adjacent siblings. This means that the second element directly follows the first, and both share the same parent. 

* **SYNTAX:** A + B
* **EXAMPLE:**  ```h1 + p``` will match all ```<p>``` elements that directly follow and ```<h2>```.
 
Question found at: https://lms.devmountain.com/courses/70/pages/first-kata-are-the-numbers-in-order?module_item_id=21638