# Saveetha_Admission_clone
## Date:9/7/2025

## Objective:
To design a landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS. This activity reinforces skills in layout design, form creation, user input handling, responsive structure, and visual styling based on a real-world example.

## Tasks:
#### 1. Analyze the Landing Page Layout:
Observe the split-screen layout with a promotional section on the left and a form on the right.

Note the use of background images, text styling, and branding elements.

#### 2. Create the HTML Structure:
Use semantic tags like ```<section>, <header>, <form>, and <footer>``` to organize content.

Structure the form with input fields such as name, email, phone, password, city, state, course, specialization, captcha, and checkbox.

#### 3. Add Form Functionality:
Include appropriate input types (text, email, tel, password, select, etc.) with placeholders and labels.

Use the <button> element for the "APPLY NOW" action.

#### 4. Apply CSS Styling:
Implement a split layout using flexbox or grid.

Style the form elements with padding, shadows, background colors, and rounded borders.

Include hover effects and button transitions to match the original look.

#### 5. Incorporate Images and Branding:
Add the institution logo and use matching fonts and colors.

Place a background image or blurred overlay behind the form content if needed.

#### 6. Ensure Responsiveness:
Make sure the page adapts to different screen sizes using media queries.

Maintain readability and layout integrity on both desktop and mobile.

## HTML Code:
```
<!-- <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Saveetha Engineering College</title>
</head>
<body>
    <div class="container-reg">
        <h3>Admission Open 2025</h3>
        <div>
            <h4>Name:</h4>
            <form>
                <input type="text" placeholder="Enter Name *" required>
                <br>
                <input type="email" placeholder="Enter Email *" required>
                <br>
                <select>
                    <option>+91</option>
                    <option>+61</option>
                </select>
                <input type="tel" placeholder="Enter Mobile Number *" required>
                <br>
                <input type="password" placeholder="Any Password of Your Choice *" required>
                <br>
                <select>
                    <option>State *</option>
                    <option >Tamilnadu</option>
                    <option>Kerala</option>
                    <option>Delhi</option>
                </select>
                <select>
                    <option>City *</option>
                    <option >Chennai</option>
                    <option>Cuddalore</option>
                    <option>Vilupuram</option>
                </select>
                <br>
                <select>
                    <option>Courses *</option>
                    <option >B.E</option>
                    <option>M.E</option>
                </select>
                <select>
                    <option>Specialization *</option>
                    <option >CSE</option>
                    <option>IT</option>
                    <option>AIDS</option>
                </select>
                <br>
                <input type="checkbox" required>
                <label>I authorise Saveetha Engineering College & its representatives to contact me with updates and notifications via Email/SMS/What'sApp/Call. This will override DND/NDNC *</label>

                <br>
                <input type="submit" placeholder="APPLY NOW">
            </form>

            <br>
            <h4>Already have an Account? Login
Resend Verification Email</h4>
        </div>
    </div>
    
</body>
</html> -->

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Saveetha College Admission</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <div class="container">
    <div class="form-box">
      <h2>Admissions Open 2025</h2>
      <form>
        <input type="text" placeholder="Enter Name *" class="name" required />
        <input type="email" placeholder="Enter Email Address *" class="name" required />
        <input type="tel" placeholder="Enter Mobile Number *" class="name" required />
        <input type="password" placeholder="Any Password of Your Choice *" class="name" required />
        
        <div class="inline-inputs">
            <select>
                    <option>State *</option>
                    <option >Tamilnadu</option>
                    <option>Kerala</option>
                    <option>Delhi</option>
                </select>
            <select>
                    <option>City *</option>
                    <option >Chennai</option>
                    <option>Cuddalore</option>
                    <option>Vilupuram</option>
                </select>
        </div>
        
        <div class="inline-inputs">
          <select>
                    <option>Courses *</option>
                    <option >B.E</option>
                    <option>M.E</option>
                </select>
                <select>
                    <option>Specialization *</option>
                    <option >CSE</option>
                    <option>IT</option>
                    <option>AIDS</option>
                </select>
        </div>
        
        <div class="inline-inputs">
          <div class="captcha">4cc915</div>
          <input type="text" placeholder="Enter Captcha" />
        </div>

        <label class="checkbox">
          <input type="checkbox" required /> I authorise Saveetha Engineering College to contact me.
        </label>

        <button type="submit" class="but">APPLY NOW ➤</button>

        <p class="login-link">
          Already have an Account? <a href="#">Login</a><br />
          <a href="#">Resend Verification Email</a>
        
        </p>
      </form>
    </div>
  </div>
</body>
</html>
```
## CSS Code:
```
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body,html{
  height: 100%;
}
.container{
  background: url(college.jpg) no-repeat center center/cover;
  height: 95vh;
  display: flex;
  justify-content: end;
  align-items: center;
  padding: 10px;
}
.form-box{
  opacity: 75%;
  width: 400px;
  background-color: rgb(32, 25, 25);
  border-radius: 12px;
  padding: 30px;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
  overflow-y: auto;
  max-height: 90vh;
}
.form-box h2{

  text-align: center;
  margin-bottom: 20px;
  color: #f5f4f4;

}
.name{
  padding: 10px;
  width: 100%;
  margin-bottom: 12px;
  border: 1px solid #ed7878;
  border-radius: 5px;
}
.inline-inputs{
  display: flex;
  margin-bottom: 12px;
  gap: 10px;
  width: 60%;
  height: 30px;
}
.captcha{
  font-weight: bold;
  background: #eee;
  padding: 10px;
  text-align: center;
  width: 100px;
  color: #000;

}
.checkbox{
  font-size: 15px;
  display: flex;
  align-items: center;
  gap: 8px;
  color: #f8f7f7;

}
.checkbox input{
  margin-bottom: 15px;
}
.but{
  width: 100%;
  height: 35px;
  background-color: orange;
  cursor: pointer;
  color: #000;
  font-weight: bold;
  font-size: 16px;
  margin-top: 10px;
  border: none;

}
.login-link{
  font-size: 15px;
  text-align: center;
  margin-top: 15px;
  color: white;
}

.but:hover{
  width: 100%;
  background-color: #f8f7f7;
}

.login-link a {
  color: orange;
}
```
## Output:
![Screenshot 2025-07-09 201813](https://github.com/user-attachments/assets/5c9e1650-8cf7-4d21-adb9-2f58c4aad572)

## Result:
A landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS is designed successfully.
