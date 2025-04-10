# **Сутра про `display: none`**  

## **Как монах Ван обнаружил пустоту в CSS**  

```text
  [div class="void"]  
   |  
   V  
  [ ]  
   ˅  
  /* Пустота занята */  
```

Монах Ван три года изучал священные стили:  

```css
.enlightenment {
  opacity: 1;
  transition: all 10s ease-in-out;
}
```  

Но однажды он случайно написал:  

```css
.void {
  display: none;
  content: "Дао";
}
```  

И исчез.  

Ученики искали его в DOM, но нашли лишь комментарий:  

```html
<!-- Здесь был Ван. Или нет? -->
```  

Тогда главный мастер объявил:  
— *«Он достиг Nirvana Mode. Теперь его `visibility: hidden`, но он везде»*.  

### **Мораль для верстальщиков:**  

1. **`display: none` — это не конец, а переход в Shadow DOM.**  
2. **Если элемент нельзя найти — значит, он стал псевдоэлементом `::after` вечности.**  
3. **Настоящий `z-index` измеряется не в пикселях, а в уровнях просветления.**  
