# Formax

> Submit Forms with Ajax

index.html

```html
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
    <script defer src="form.js"></script>
    <script defer src="main.js"></script>
</head>
<body>
    <form id="getDog" action="https://dog.ceo/api/breeds/image/random" method="GET">
            <button>Get Dogs</button>
    </form>
</body>
</html>
```

main.js

```js
registerForm("form#getDog", async res => {
  console.log(await res.json());
});
```
