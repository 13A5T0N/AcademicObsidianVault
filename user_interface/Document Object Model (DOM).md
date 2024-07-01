### Belangrijke Concepten

1. **Document**: Het hoofdobject dat het HTML-document vertegenwoordigt.
2. **Element**: Een enkele HTML-tag binnen het document.
3. **Node**: Elk onderdeel van het document, inclusief elementen, tekst en opmerkingen.
4. **Attribute**: Eigenschappen van een element, zoals `id`, `class`, etc.

- **`document.getElementById(id)`**: Retourneert het element met de opgegeven ID.
    ```js
    var element = document.getElementById('myId');
    ```
- **`document.getElementsByClassName(className)`**: Retourneert een live HTMLCollection van elementen met de opgegeven klasse.
```js
    var elements = document.getElementsByClassName('myClass');
```
- **`document.getElementsByTagName(tagName)`**: Retourneert een live HTMLCollection van elementen met de opgegeven tagnaam.
```js
var elements = document.getElementsByTagName('div');
```
- **`document.querySelector(selector)`**: Retourneert het eerste element dat overeenkomt met de opgegeven CSS-selector.
```js
var element = document.querySelector('.myClass');
```
 
- **`document.querySelectorAll(selector)`**: Retourneert een NodeList van elementen die overeenkomen met de opgegeven CSS-selector.
    ```js
   var elements = document.querySelectorAll('.myClass'); 
```


#### Manipuleren van Elementen

- **`element.innerHTML`**: Stelt de HTML-inhoud van een element in of retourneert deze.
    
    ```js
    element.innerHTML = '<p>Nieuwe inhoud</p>';
```
 
- **`element.textContent`**: Stelt de tekstinhoud van een element in of retourneert deze.
    ```js
    element.textContent = 'Nieuwe tekst';
```

- **`element.setAttribute(name, value)`**: Stelt een attribuut in op een element.
```js
element.setAttribute('class', 'newClass');
```
- **`element.getAttribute(name)`**: Retourneert de waarde van het opgegeven attribuut.
    ```js
    var className = element.getAttribute('class');
```
- **`element.removeAttribute(name)`**: Verwijdert het opgegeven attribuut van een element.
    ```js
    element.removeAttribute('class');
```
- **`element.classList.add(className)`**: Voegt een klasse toe aan het element.
    ```js
     element.classList.add('newClass');
```
- **`element.classList.remove(className)`**: Verwijdert een klasse van het element.
    ```js
    element.classList.remove('oldClass');
```

- **`element.classList.toggle(className)`**: Voegt een klasse toe als deze niet bestaat, of verwijdert deze als deze wel bestaat.
    ```js
    element.classList.toggle('active');
```
    
    