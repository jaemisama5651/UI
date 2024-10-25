# 버튼#1

## 개요
- 기본적인 버튼을 생성하고 `hover`와 `active` 추가하여 반응적인 버튼을 만든다

- `hover`시 효과 더 진한 배경색과 `box-shadow`

## 폴더 구조
```
button/
│
├── index.html 
└── style.css  
```
## 코드
`index.html`
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Button Creation</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <button class="btn btn-basics">버튼</button>
</body>
</html>
```
<br>


`style.css`
```css
/* 기본 버튼 스타일 */
.btn {
    font-size: 16px;
    border: none;
    padding: 12px 24px;
    cursor: pointer;
    border-radius: 8px;
}

/* 기본 상태 - 검정색 계열 버튼 */
.btn-basics {
    background-color: #444;
    color: white;
    transition: all 0.3s ease;
}

/* Hover 상태 - 색상 변경 및 그림자 추가 */
.btn-basics:hover {
    background-color: #333;
    box-shadow: 4px 4px 8px rgba(0, 0, 0, 0.4);
}

/* Active 상태 - 눌림 효과 및 그림자 변경 */
.btn-basics:active {
    background-color: #222;
    transform: scale(0.95);
    box-shadow: 4px 4px 10px rgba(0, 0, 0, 0.5);
}
```

