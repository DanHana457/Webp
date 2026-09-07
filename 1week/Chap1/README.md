# HTML5 실습문제

## 문제 1

HTML5 페이지에서 **HTML 태그 2개와 CSS 1개의 오류**를 찾아 수정한다.

### 오류

1. `<DOCTYPE html>` → `<!DOCTYPE html>`
2. `</style>` 추가
3. `color = blue;` → `color: blue;`

### 최종 코드

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>오류를 찾으세요</title>
    <style>
        h3 {text-align: center; color: darkred;}
        span {color: blue; font-size: 20px;}
    </style>
</head>
<body>
<h3>Elvis Presley</h3>
He was an American singer and actor. In November 1956,
he is often referred to as "<span>the King of Rock and Roll</span>"
</body>
</html>
```

---

## 문제 2

### 오류 3개

| 구분   | 원래 코드            | 수정 코드             |
| ---- | ---------------- | ----------------- |
| HTML | `<DOCTYPE html>` | `<!DOCTYPE html>` |
| HTML | `</style>` 없음    | `</style>` 추가     |
| CSS  | `color = blue;`  | `color: blue;`    |

### 최종 코드

```html
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <title>오류를 찾으세요</title>
    <style>
        h3 { text-align: center; color: darkred; }
        span { color: blue; font-size: 20px; }
    </style>
</head>
<body>
    <h3>Elvis Presley</h3>
    He was an American singer and actor. In November 1956,
    he is often referred to as "<span>the King of Rock and Roll</span>"
</body>
</html>
```

---

## 문제 3

### 요구사항

* `<span>` 글자색을 `violet`으로 변경
* `<hr>` 두께를 `10px`로 변경

```css
span {
    color: violet;
}

hr {
    height: 10px;
    background-color: black;
    border: 0;
}
```

```html
<h3>Elvis Presley</h3>
<hr>

He was an American singer and actor. In November 1956,
he made his film debut in <span>Love Me Tender</span>.
He is often referred to as "the King of Rock and Roll".
```

---

## 문제 4

### 마우스를 올리면 사진 변경

`Love Me Tender`에 마우스를 올리면 사진이 변경된다.

```html
<img id="photo" src="elvis.jpg" alt="Elvis Presley 사진">

<p>
    He made his film debut in
    <span
        onmouseover="document.getElementById('photo').src='myphoto.jpg'"
        onmouseout="document.getElementById('photo').src='elvis.jpg'">
        Love Me Tender
    </span>.
</p>
```
