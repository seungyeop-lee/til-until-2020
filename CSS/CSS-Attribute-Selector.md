# 속성 선택자

- 특정 속성을 가지고 있는 요소를 선택하는 속성 선택자에 대해 정리한다.
- 속성 선택자는 단독으로도 사용 가능하지만, 태그를 나타내는 선택자와도 같이 사용 가능하다.
  - `태그[속성]` 형태로 사용

## `[속성]` 선택자

- 지정한 속성과 같은 속성을 가지고 있는 요소 전부를 선택한다.

```css
p[class] {
  /* <p>태그 중 class 속성을 가지고 있는 모든 요소를 선택 */
}
```

## `[속성 = 값]` 선택자

- 지정한 속성의 속성값이 지정한 값과 같은 요소 전부를 선택한다.

```css
p[id=news-contents] {
  /* <p>태그 중 id속성에 news-contents라는 값을 가지고 있는 
  모든 요소를 선택 */
}
```

## `[속성 ~= 값]` 선택자

- 지정한 속성의 속성 값 중 지정한 값이 포함(단어별)되어 있는 요소 전부를 선택한다.

```css
p[class~=subject] {
  /* <p>태그 중 class속성에 subject라는 값을 포함한 
  요소 전부를 선택한다. */
}
```

## `[속성 |= 값]` 선택자

- 지정한 속성의 속성 값 중 지정한 값이 포함(하이픈 포함 단어별)되어 있는 요소 전부를 선택한다.

```css
p[class|=subject] {
  /* <p>태그 중 class속성에 subject라는 값을 포함한 
  요소 전부를 선택한다. */
}
```

## `[속성 ^= 값]` 선택자

- 지정한 속성의 속성 값 중 지정한 값으로 시작하는 요소 전부를 선택한다.

```css
p[class^=subject] {
  /* <p>태그 중 class속성에 subject라는 값으로 시작하는 
  요소 전부를 선택한다. */
}
```

## `[속성 $= 값]` 선택자

- 지정한 속성의 속성 값 중 지정한 값으로 끝나는 요소 전부를 선택한다.

```css
p[class~=subject] {
  /* <p>태그 중 class속성에 subject라는 값으로 끝나는 
  요소 전부를 선택한다. */
}
```

## `[속성 *= 값]` 선택자

- 지정한 속성의 속성 값 중 지정한 값이 속성 값의 일부인 요소 전부를 선택한다.

```css
p[class~=a] {
  /* <p>태그 중 class속성의 속성 값 중 a가 일부를 이루고 있는 
  요소 전부를 선택한다. */
}
```

## 참고

- [Do it! HTML5+CSS3 웹 표준의 정석 <개정판>, 2017, 고경희](http://www.easyspub.co.kr/20_Menu/BookView/119/PUB)