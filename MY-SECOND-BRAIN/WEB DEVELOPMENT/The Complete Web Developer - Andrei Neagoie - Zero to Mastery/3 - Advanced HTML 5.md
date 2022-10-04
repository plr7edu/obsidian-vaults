# Html Forms

```html
<!DOCTYPE html>
<html>
<head>
	<titel>Register Page</titel>
	</head>
<body>
	<h1>Register Page</h1>
	<!-- USE POST NOT GET -->
	<div>
		<form method="POST">
			 First Name: <input type="text" name="firstname"><br>
			 Last Name: <input type="text" name="Secondname"><br>
			 Email : <input type="email" name="email" required><br>
			 Password : <input type="password" name="password" min="12"> <br>
			 Birthday : <input type="date" name="birthday" ><br>
			 Gender : <br>
			 <input type="radio" name="Gender" value="male" >Male<br>
			 <input type="radio" name="Gender" value="female" >Female<br>
			 <input type="radio" name="Gender" value="other" >Other<br>
			 Pets : <br>
			 <input type="checkbox" name="dog">Dog <br>
			 <input type="checkbox" name="cat" >Cat <br>
			 <input type="checkbox" name="fish" >Fish <br>
			 Cars : <br>
			 <select>
			 	<option value="Audi" name="audi">Audi</option>
			 	<option value="Volvo" name=Volvo >Volvo</option>
			 </select> <br>
			 <input type="submit" value="Register">
			 <input type="reset">
		</form>
	</div>
	<a href="index.html"><p>Back</p></a>
	
</body>
</html> 
```



<!DOCTYPE html>
<html>
<head>
	<titel>Register Page</titel>
	</head>
<body>
	<h1>Register Page</h1>
	<!-- USE POST NOT GET -->
	<div>
		<form method="POST">
			 First Name: <input type="text" name="firstname"><br>
			 Last Name: <input type="text" name="Secondname"><br>
			 Email : <input type="email" name="email" required><br>
			 Password : <input type="password" name="password" min="12"> <br>
			 Birthday : <input type="date" name="birthday" ><br>
			 Gender : <br>
			 <input type="radio" name="Gender" value="male" >Male<br>
			 <input type="radio" name="Gender" value="female" >Female<br>
			 <input type="radio" name="Gender" value="other" >Other<br>
			 Pets : <br>
			 <input type="checkbox" name="dog">Dog <br>
			 <input type="checkbox" name="cat" >Cat <br>
			 <input type="checkbox" name="fish" >Fish <br>
			 Cars : <br>
			 <select>
			 	<option value="Audi" name="audi">Audi</option>
			 	<option value="Volvo" name=Volvo >Volvo</option>
			 </select> <br>
			 <input type="submit" value="Register">
			 <input type="reset">
		</form>
	</div>
	<a href="index.html"><p>Back</p></a>
	
</body>
</html> 


# HTML `<div>` Tag

The `<div>` tag defines a division or a section in an HTML document.

The `<div>` tag is used as a container for HTML elements - which is then styled with CSS or manipulated with JavaScript.

The `<div>` tag is easily styled by using the class or id attribute.

Any sort of content can be put inside the `<div>` tag!


# HTML `<span>` Tag

The `<span>` tag is an inline container used to mark up a part of a text, or a part of a document.

The `<span>` tag is easily styled by CSS or manipulated with JavaScript using the class or id attribute.

The `<span>` tag is much like the`<div>` element, but `<div>` is a block-level element and `<span>` is an inline element.

```html
<!DOCTYPE html>
<html>
<body>

<h1>The span element</h1>

<p>My mother has <span style="color:blue;font-weight:bold">blue</span> eyes and my father has <span style="color:darkolivegreen;font-weight:bold">dark green</span> eyes.</p>

</body>
</html>

```

<!DOCTYPE html>
<html>
<body>

<h1>The span element</h1>

<p>My mother has <span style="color:blue;font-weight:bold">blue</span> eyes and my father has <span style="color:darkolivegreen;font-weight:bold">dark green</span> eyes.</p>

</body>
</html>


