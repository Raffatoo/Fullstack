### Nueva Nota [+](https://studies.cs.helsinki.fi/exampleapp/notes): 

> Formularios y HTTP POST, flujo para agregar una nueva nota:

sequenceDiagram
Usuario->>Navegador: Abre Navegacion
Navegador->>Servidor: GET URL 
Usuario->>Navegador: Nueva Nota
loop Escribir Nota
    Usuario->>Usuario: Nueva Nota Escrita
end
Usuario->>Navegador: Guardar
Navegador->>Servidor: POST Nueva Nota
Navegador->>Servidor: GET URL
Usuario-->>Navegador: Cierra Navegacion




sequenceDiagram
Alice->>John: Hello John, how are you?
loop Healthcheck
    John->>John: Fight against hypochondria
end
Note right of John: Rational thoughts!
John-->>Alice: Great!
John->>Bob: How about you?
Bob-->>John: Jolly good!

https://www.mermaidchart.com/raw/893ef463-8d5d-4a1f-a23a-b97108780e02?theme=light&version=v0.1&format=svg


classDiagram
    Animal <|-- Duck
    Animal <|-- Fish
    Animal <|-- Zebra
    Animal : +int age
    Animal : +String gender
    Animal: +isMammal()
    Animal: +mate()
    class Duck{
      +String beakColor
      +swim()
      +quack()
    }
    class Fish{
      -int sizeInFeet
      -canEat()
    }
    class Zebra{
      +bool is_wild
      +run()
    }












### Supercharging the React ecosystem via [TanStack](https://tanstack.com) with projects and products like:
- 🤖 TanStack Query
- 🤖 TanStack Table
- 🤖 TanStack Router
- 🤖 TanStack Start
- 🤖 TanStack Virtual
- 🤖 TanStack Form
- ⚛️ React Charts
- 🏊‍♂️ Swimmer JS

> Previously 📊 Chart.js, ⚛️ React Static and 🔀 Crossfilter

---

Hello! I build open source software that is currently used by hundreds of thousands of developers at companies ranging from fortune 500 companies like Apple, Google, Facebook, Amazon, Netflix, Walmart, and Target all the way down to startups and indie developers.

Most of my open source software is written in Javascript and focused on Headless UI, State Management, Data Viz, and Enterprise Application Architecture.

### For Developers

By helping your company become a Github Sponsor, you will not only feel great about giving back to the open source tools that run your business, but also get some awesome perks! Each of the sponsorship tiers on this page have their perks listed on them. If you believe your company could become a sponsor, then please reach out!

### For Companies and Businesses

By becoming a Github Sponsor, your company and brand will be recognized as a one that gives back to the open source tools that run your business and one that respects your developers time and your customers' experience. You also receive premium perks based on your sponsorship tier for things like free advertising on my web properties, free course vouchers, exclusive access to private repos and tools, free consultation hours with yours truly, and even on-demand support!

### Perks


#### .start(tour)
- Starts a Tour
- Params:
  *	*tour*: Tour Object
- Returns:
  *	Promise that resolves when the tour is finished or rejected when aborted.

#### .stop()
- Stops a Tour
- Returns:
  *	Promise that resolves when the tour is stopped.

#### .next()
- Goes to the next step in the current tour
- Returns:
  *	Promise that resolves when the next step is reached

#### .previous()
- Goes to the previous step in the current tour
  *	Promise that resolves when the previous step is reached

#### .goto(index)
- Goes to a specific step in the tour
- Params:
  *	*index*: The 0-index number of the step eg. `0, 1, 2, 3`

- Returns:
  *	Promise that resolves when the specific step is reached


## Using Promise Event Hooks
You can pass any function that returns a promise to the `before` and `after` properties for any step.  When the promise resolves, the tour moves on accordingly.

#### Example
```javascript
var tour = {
	steps: [{
      target: '#first-element',
      content: 'This is the first step!',
    }, {
      target: '.some .other .element',
      content: 'Blah blah blah.',
      before: () => {
      	// Do something amazing
      	return new Promise()
    	}
    }, {
      target: '#menu-element',
      content: 'I guess this is a menu!',
      after: () => {
      	// Do some more cool stuff
      	return new Promise()
    	}
    }, {
      target: '#last-element',
      content: 'It is over! :(',
    }]
}
```


# Tour

A simple, minimalist touring and on-boarding library for javascript

[![](https://avatars0.githubusercontent.com/u/20192755?v=3&s=500)](http://tourjs.github.io/tour)

[![Join the chat at https://gitter.im/tourjs/tour](https://badges.gitter.im/tourjs/tour.svg)](https://gitter.im/tourjs/tour?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

## [Awesome Demo](http://tourjs.github.io/tour)

## Features

* Supports single page apps, and complex scrollable content
*	Responsive & Intelligent
*	Automagic Positioning
*	Promise Driven Events & Hooks
*	Tour does not manipulate or relayer your DOM elements in any way