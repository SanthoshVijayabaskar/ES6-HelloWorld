# Hello World Program :pray:

<h5>STEP 1: Setup Babel CommandLine Utility [https://babeljs.io/docs/setup/]</h5>
```
npm install -g babel-cli
```
<h5>STEP 2: Install Babel Preset for ES2015</h5>
```
npm install babel-preset-es2015
```
<h5>STEP 3: Create .babelrc File </h5>
```
{
    "presets": [
        "es2015"
    ]
}
```
<h5>STEP 4: Create Project Structure </h5>
```
-dist
-src
 - main.js
-index.html
```
<h5>STEP 5: index.html</h5>
``` html
<!doctype html>
<html>
	<head>
		<meta charset="utf-8">
		<title>ES6 Hello World</title>
		<meta name="description" content="An example of how to use ES6 with the Babel transpiler">
		<meta name="viewport" content="width=device-width, initial-scale=1">
	</head>
	<body>
		<p>Welcome to Getting Started with JavaScript 6 Webinar<p>

		<script src="dist/main.js"></script>
	</body>
</html>
```

<h5>STEP 6: main.js</h5>
``` javascript
let greeting = `hello world`;
console.log(greeting);
```
<h5>STEP 7: Run the Babel Transpilation and Check the Output</h5>
```
babel src --out-dir dist --source-maps
```
<p>Why Source-Maps? Demo: http://www.thecssninja.com/demo/source_mapping/</p>