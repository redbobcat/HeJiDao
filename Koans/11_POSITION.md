# **Притча про `position: absolute`**  

## **Как монах Чжан вышел из потока**  

Монах Чжан всегда использовал:  

```css  
.ego {  
  position: relative;  
}  
```  

Но однажды он обнаружил, что застрял в `overflow: hidden` жизни. Тогда он написал:  

```css  
.enlightenment {  
  position: absolute;  
  top: unset;  
  bottom: unset;  
  left: calc(50% - ∞px);  
}  
```  

И исчез из DOM.  

Ученики искали его в DevTools, но единственным следом был комментарий:  

```html  
<!-- Чжан теперь в stacking context вселенной -->  
```  

### **Мораль:**  

1. **`fixed` — для слабаков.** Настоящие мастера используют `position: cosmic`.  
2. **Если `z-index` не работает — значит, ты ещё в родительском контейнере.**  
3. **Координата `left: 50%` бесполезна без `transform: translateX(-50%)` смирения.**  
