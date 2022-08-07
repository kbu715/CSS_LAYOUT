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
- [ ] grid-template-areas
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