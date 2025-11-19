  

HTML forms are used to collect information from users.

Example: login forms, contact forms, search bars, sign-up pages, etc.

### 1️⃣ Basic Form Structure

A form is created using the `<form>` tag.
```html
<form action="/submit" method="POST">

<!-- form fields go here -->

</form>
```

What these mean:
	- action → where the data will be sent
	- method → how the data will be sent
	- GET → visible in URL (used for search)
	- POST → hidden (used for password, login, etc.)

2️⃣ Text Input
Used for simple text like names.
```html
<form>

	<label>Full Name:</label>

	<input type="text" name="fullname">

</form>
```

Notes:
- label gives a title.
- input collects data.
- name is the variable name sent to the server.

3️⃣ Email Input

HTML validates the email automatically.

```Html

<form>

	<label>Email:</label>

	<input type="email" name="email">

</form>
```

4️⃣ Password Input

Text is hidden with dots:
```html
<form>

	<label>Password:</label>
	<input type="password" name="password">

</form>
```

5️⃣ Number Input

```html
<form>

	<label>Age:</label>

	<input type="number" name="age" min="1" max="120">

</form>
```

6️⃣ Textarea (Multi-line text)

Used for long messages, comments, descriptions.
```html
<form>

	<label>Message:</label><br>

	<textarea name="message" rows="4" cols="30"></textarea>

</form>
```

7️⃣ Radio Buttons (Choose ONE option)

Example: choose gender.
```html
<form>

<p>Gender:</p>

	<input type="radio" name="gender" value="male"> Male<br>

	<input type="radio" name="gender" value="female"> Female<br>

</form>
```

Note:
- All radio buttons must share the same name.

8️⃣ Checkboxes (Choose MANY options)

Example: select skills.
```html
<form>
<p>Skills:</p>
	<input type="checkbox" name="skill_html"> HTML<br>
	<input type="checkbox" name="skill_css"> CSS<br>
	<input type="checkbox" name="skill_js"> JavaScript<br>
</form>
```

9️⃣ Dropdown (Select Menu)
```html
<form>
	<label>Country:</label>
	<select name="country">
	<option value="ng">Nigeria</option>
	<option value="gh">Ghana</option>
	<option value="us">USA</option>
</select>
</form>
```

🔟 Submit Button

```html
<form>
<input type="submit" value="Submit">
</form>
```