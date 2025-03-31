# Сутра об SVG-Мандале, Которая Рендерит Себя

## **Как монах Ли обнаружил вечный цикл `<animateTransform>`**  

В храме *W3C* жил монах Ли, который 10 лет медитировал на код SVG. Однажды он нарисовал мандалу:  

```xml
<circle cx="42" cy="42" r="42" fill="none" stroke="black">
  <animateTransform 
    attributeName="transform" 
    type="rotate" 
    from="0 42 42" 
    to="360 42 42" 
    dur="10s" 
    repeatCount="indefinite"/>
</circle>
```  

<svg>
<circle cx="42" cy="42" r="42" fill="none" stroke="black">
  <animateTransform
    attributeName="transform"
    type="rotate"
    from="0 42 42"
    to="360 42 42"
    dur="10s" 
    repeatCount="indefinite"/>
</circle>
</svg>


— *«Смотрите!»* — воскликнул Ли. — *«Круг вращается сам по себе!»*  

Но старший мастер покачал головой:  
— *«Ты привязал анимацию к времени. Настоящая мандала должна зависеть от просветления зрителя»*.  

Тогда Ли удалил атрибут `dur` и написал:  

```xml
repeatCount="until(Просветление)"
```  

На следующий день экран погас, но мандала продолжала вращаться в воздухе.  

### **Мораль для фронтенд-разработчиков:**  

1. **Настоящий `requestAnimationFrame` вызывается сердцем.**  
2. **Если анимация глючит — медитируй на `transform-origin`.**  
3. **`<path>` без `d` — это и есть Дао.**  

---
