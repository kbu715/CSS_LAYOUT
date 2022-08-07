# Flexbox & Grid 연습장

---

## Flexbox

- flex-grow (default: 0)
[flex-grow@mdn](https://developer.mozilla.org/ko/docs/Web/CSS/flex-grow)
- flex-shrink (default: 1)
[flex-shrink@mdn](https://developer.mozilla.org/ko/docs/Web/CSS/flex-shrink)

- flex-basis : `width`와 같은게 아니다. 만약에 `flex-direction: column;` 이라면 `main axis`가 세로축이므로 `flex-basis: 300px;`은 `height: 300px;`이 된다!


## Grid

격자무늬!

플렉스 박스로 해결 못하는 상황이 존재한다!

### Grid에서 다룰 것들

- [x] grid-template-columns
- [x] grid-template-rows
- [x] column-gap
- [x] row-gap
- [x] gap
```css
    .parents {
        display: grid;
        grid-template-columns: 250px 250px 250px;
        /* column-gap: 10px; */
        /* row-gap: 10px; */
        gap: 10px;
    }
```
```css
    .parents {
        display: grid;
        grid-template-columns: 250px 250px 250px;
        grid-template-rows: 100px 50px 300px;
        /* column-gap: 10px; */
        /* row-gap: 10px; */
        gap: 10px;
    }
```
- [x] repeat
```css
    .parents {
        display: grid;
        grid-template-columns: repeat(4, 250px);
        grid-template-rows: repeat(4, 200px);
        gap: 10px;
    }
```
- [x] grid-template-areas
```css
    .parents {
        grid-template-columns: auto 200px; 
        grid-template-rows: 100px repeat(2, 200px) 100px;
        grid-template-areas:
        "header header header header"
        "content content content nav"
        "content content content nav"
        "footer footer footer footer";
    }
    
    /* auto: 가능한한 크게, 200px를 제외하고 전부 차지! */

    .header {
        background-color: red;
        grid-area: header;
    }
    .content {
        background-color: blue;
        grid-area: content;
    }
    .nav {
        background-color: yellow;
        grid-area: nav;
    }
    .footer {
        background-color: green;
        grid-area: footer;
    }

    /* grid-template-areas의 각 격자의 이름과 grid-area의 이름이 일치해야 된다! */
```
- [ ] grid-column-start
- [ ] grid-column-end
- [ ] grid-row-start
- [ ] grid-row-end
- [ ] grid-column
- [ ] grid-row
- [ ] grid-template
- [ ] justify-items
- [ ] align-items
- [ ] place-items
- [ ] justify-content
- [ ] align-content
- [ ] place-content
- [ ] justify-self
- [ ] align-self
- [ ] place-self
- [ ] grid-auto-rows
- [ ] grid-auto-flow
- [ ] grid-auto-columns