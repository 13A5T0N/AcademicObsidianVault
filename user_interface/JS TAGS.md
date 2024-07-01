
### HTML Elements for JavaScript

1. **`<script>`**: Dit element wordt gebruikt om JavaScript in een HTML-document op te nemen.
    
    - **`src`**: Specificeert een externe JavaScript-bestand.
    - **`type`**: Geeft het type script aan, meestal `text/javascript`.
    - **`async`**: Voert het script asynchroon uit.
    - **`defer`**: Stelt de uitvoering van het script uit tot na het parsen van de HTML.
```js
<!-- Inline JavaScript --> 
<script>   console.log('Hello, world!'); </script> 
<!-- External JavaScript --> 
<script src="script.js"></script>  
<!-- Async External JavaScript --> 
<script src="script.js" async></script>  
<!-- Defer External JavaScript --> 
<script src="script.js" defer></script>
```
    
**`<noscript>`**: Dit element geeft inhoud weer voor gebruikers die geen JavaScript hebben ingeschakeld of wanneer de browser geen JavaScript ondersteunt.
```js
<noscript>   
	JavaScript is disabled in your browser. Please enable it to view this content </noscript>
```

### Event Attributes

HTML-elementen kunnen verschillende attributen hebben die JavaScript-functies aanroepen als bepaalde gebeurtenissen plaatsvinden. Enkele van de meest voorkomende gebeurtenissen zijn:

- **`onclick`**: Wordt aangeroepen wanneer een element wordt aangeklikt.
```js
<button onclick="alert('Button clicked!')">Click me</button>    
```
- **`onload`**: Wordt aangeroepen wanneer een pagina of een afbeelding volledig is geladen.
```js
  <body onload="init()">  
```
- **`onchange`**: Wordt aangeroepen wanneer de waarde van een invoerelement verandert.
```js
    <input type="text" onchange="handleChange(this)">
```
- **`onmouseover`**: Wordt aangeroepen wanneer de muis over een element beweegt.
```js
    <div onmouseover="hoverEffect(this)">
```
- **`onmouseout`**: Wordt aangeroepen wanneer de muis een element verlaat.
```js
<div onmouseout="removeHoverEffect(this)">    
```
- **`onkeyup`**: Wordt aangeroepen wanneer een toets wordt losgelaten.
```js
    <input type="text" onkeyup="handleKeyUp(event)">
```
- **`onfocus`**: Wordt aangeroepen wanneer een element de focus krijgt.
```js
<input type="text" onfocus="handleFocus(this)">
```    
- **`onsubmit`**: Wordt aangeroepen wanneer een formulier wordt ingediend.
 ```js
 <form onsubmit="return validateForm()">
```  
