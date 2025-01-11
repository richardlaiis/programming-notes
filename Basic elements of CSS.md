```html
<!DOCTYPE html>
<html lang="zh-Hant-TW">
	<head>
		<meta charset="UTF-8">
		<title>hi</title>
		<meta name="description" content="Useless site, like my whole life">
		<!--So that search engines can pick up this description to show with the results of searches-->
		<link rel="stylesheet" href="style.css">
		<!--import web fonts (Google font)-->
		<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
		<link href="https://fonts.googleapis.com/css2?family=Cactus+Classical+Serif&family=Noto+Serif+TC:wght@200..900&display=swap" rel="stylesheet">
	</head>
	<body>
		<h1>
		header 1
		</h1>
		<p>lorem ipsum</p>
	</body>
</html>
```
## imporkt

```html
<link rel="stylesheet" href="style.css">
```
## font

```css
/*style.css*/
p {
	font-size: 0.5rem; /*0.5 * size of the "parent element", px, %*/
	text-align: justify; /*左右對齊是justify, center right left*/
	line-height: 1.7;
	font-weight: bold; /*normal, lighter, bolder*/
	font-family: "Cactus Classical Serif", serif;
}
```

## grid

```css
.container {
	display: grid;
	grid-template-columns: 1fr 1fr 1fr;
	gap: 15px;
}
.item {
	background: #FAFFC5;
	color: #3A3960;
	padding: 10px;
}

```