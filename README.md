<HTML>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Name Field</title>
<style>
  ::placeholder {
    color: lightgray;
  }
</style>
</head>
<h1> Sign up </h1>
<body>
<form>
<label for="name">Name:</label><br>
  <input type="text" id = "name" placeholder="full name">
<br><br>
<lable for="email">email:</lable><br>
   <input type="email" id="email" name="email" placeholder="gmail id">
<br><br>
<lable for="psw">Password:</lable><br>
   <input type="password" id="psw" name="psw" placeholder="8 characters">
<br><br>
<label>Confirm Password:</lable><br>
    <input type="password" name = confirm_password" placeholder="8 characters" required>
<br><br>
<lable>Date Of Birth:</lable><br>
    <input type="date">
<br><br>
<lable for="gender">Gender:</lable><br>
    <input type="radio" id="male" name="gender" value="Male">
    <lable for="male">Male</lable>
    <input type="radio" id="female" name="gender" value="Female">
    <lable for="female">Female</lable> 
    <input type="radio" id="other" name="gender" value="Other">
    <lable for="other">Other</lable>
<br><br>
<lable for="photo">Insert your photo:</lable><br>
   <input type="file" id="photo" name="photo" accept="image/*" placeholder="No file chosen">
<br><br>
<label for="document">Insert Resume:</label><br>
   <input type="file" id="document" name="document" accept=".doc, .docx, .pdf" placeholder="No file chosen">
<br><br>
<label for="security_question">Security Question:</label><br>
   <select id="security_question" name="security_question">
    <option value="q1">What is your mother's maiden name?</option>
    <option value="q2">What city were you born in?</option>
    <option value="q3">What is your favorite book?</option>
    <option value="q4">What is the name of your first pet?</option>
   </select>
   <br><br>
   <label for="security_answer">Your answer:</label>
   <input type="text" id="security_answer" name="security_answer" required>
<br><br>
<input type="checkbox">
<label>I agree to terms and conditions</lable><br>
<button type="submit">Register</button>
</form>
</body>
     </html>
