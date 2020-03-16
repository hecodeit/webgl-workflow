# workflow
https://mattdesl.svbtle.com/rapid-prototyping

## init project
```
mkdir my_project
cd  my_project
npm init -y

npm install budo browserify uglify-js --save-dev
touch demo.js
```

```
"start": "budo demo.js:bundle.js --live",
"build": "browserify demo.js | uglifyjs -cm > bundle.js"
```

## html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>my-module</title>
</head>
<body>
    <script src="bundle.js"></script>
</body>
</html>
```

## git

```
git init
git remote add origin git@github.com:hecodeit/webgl-workflow.git
git fetch

git add.
git commit -m 'updating build'
git push origin master
```
