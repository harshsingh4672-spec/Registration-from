# Registration-from
A simple registration form using HTML and CSS
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Registration Form</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, sans-serif;
}

body{
    background:linear-gradient(135deg,#4facfe,#00f2fe);
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
}

.container{
    background:#fff;
    width:400px;
    padding:25px;
    border-radius:12px;
    box-shadow:0 5px 15px rgba(0,0,0,0.3);
}

h2{
    text-align:center;
    margin-bottom:20px;
    color:#333;
}

input,
select,
textarea{
    width:100%;
    padding:10px;
    margin:8px 0 15px;
    border:1px solid #ccc;
    border-radius:5px;
}

.gender{
    margin-bottom:15px;
}

.gender input{
    width:auto;
}

button{
    width:100%;
    padding:12px;
    background:#007BFF;
    color:white;
    border:none;
    border-radius:5px;
    cursor:pointer;
    font-size:16px;
}

button:hover{
    background:#0056b3;
}
</style>

</head>
<body>

<div class="container">

<h2>Registration Form</h2>

<form action="https://api.web3forms.com/submit" method="POST">

<input type="hidden" name="access_key" value="YOUR_ACCESS_KEY">

<label>Full Name</label>
<input type="text" name="name" required>

<label>Email</label>
<input type="email" name="email" required>

<label>Phone</label>
<input type="tel" name="phone" required>

<label>Password</label>
<input type="password" name="password" required>

<label>Date of Birth</label>
<input type="date" name="dob">

<label>Gender</label>

<div class="gender">
<input type="radio" name="gender" value="Male"> Male
<input type="radio" name="gender" value="Female"> Female
<input type="radio" name="gender" value="Other"> Other
</div>

<label>Country</label>

<select name="country">
<option>India</option>
<option>USA</option>
<option>Canada</option>
<option>Australia</option>
</select>

<label>Address</label>

<textarea name="address" rows="4"></textarea>

<button type="submit">Register Now</button>

</form>

</div>

</body>
</html>
