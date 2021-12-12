<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="assignment.css" />
</head>
<body>
    <div class="title-container">
        <h2 class="ubuntu-font">Admission Form For Geekster</h2>
    </div>
    <div class="form-container">
        <form>
            <h4 class="roboto-font">Personal Info</h4>
            <input type="text" class="inline m-4" name="f_name" placeholder="First Name" autocomplete="off" required/>
            <input type="text" class="inline m-4" name="l_name" placeholder="Last Name" autocomplete="off"/>
            <br />
            <input type="email" class="inline m-4" name="mail" placeholder="Email ID" autocomplete="off" required/>
            <br />
            <input type="tel" class="inline m-4" name="phone" placeholder="Phone Number" autocomplete="off" required pattern="[0-9]{4}-[0-9]{3}-[0-9]{3}" title="Please enter in the format 1111-111-111"/>
            <br />
            <input class="inline m-4" type="date" name="date_of_birth" max="2022-01-01" />
            <br />
            <select class="inline m-4" name="gender">
                <option selected disabled>Select Gender</option>
                <option>Male</option>
                <option>Female</option>
                <option>Other</option>
            </select>
            <br />
            <textarea name="address" placeholder="Address" class="m-4"></textarea>
            <hr />
            <h4 class="roboto-font">Education Info</h4>
            <select name="degree" class="inline m-4">
                <option selected disabled>Select Degree</option>
                <optgroup label="Bachelors">
                    <option>B. Tech</option>
                    <option>B.E.</option>
                    <option>B. Sc.</option>
                </optgroup>
                <optgroup label="Masters">
                    <option>M. Tech</option>
                    <option>M.E.</option>
                    <option>M. Sc.</option>
                </optgroup>
            </select>
            <br />
            <input type="text" name="college" class="inline m-4" placeholder="College Name" />
            <br />
            <input type="text" name="graduation_year" class="inline m-4" placeholder="Year of graduation" min="2010" max="2022" />
            <br />
            <input type="text" name="percentage" class="inline m-4" placeholder="Percentage" min="0" max="100" step="0.1" />
            <br />
            <h4 class="roboto-font">class X Details</h4>
            <input type="text" name="classX_BOARD" class="inline m-4" placeholder="School Name" />
            <br />
            <input type="text" name="classXPassout_year" class="inline m-4" placeholder="Year of Passout" min="2010" max="2018" />
            <br />
            <input type="text" name="percentage" class="inline m-4" placeholder="Percentage" min="0" max="100" step="0.1" />
            <br />
            <h4 class="roboto-font">class XII Details</h4>
            <input type="text" name="classXII_BOARD" class="inline m-4" placeholder="School Name" />
            <br />
            <input type="text" name="classXIIPassout_year" class="inline m-4" placeholder="Year of Passout" min="2010" max="2018" />
            <br />
            <input type="text" name="percentage" class="inline m-4" placeholder="Percentage" min="0" max="100" step="0.1" />
            <br />




            <h5 class="inline roboto-font">Upload Resume: </h5>
            <input type="file" class="inline m-4" />
            <hr />
            <h4 class="roboto-font">Course Details</h4>
            <p class="roboto-font">Which level do you want to enroll?</p>
            <input type="radio" class="m-4" name="course_type" /><span class="roboto-font">Fundamentals</span>
            &emsp;&emsp;
            <input type="radio" class="m-4" name="course_type" /><span class="roboto-font">Advanced</span>
            <br />
            <br />
            <p class="roboto-font">Which course do you want to enroll?</p>
            <input type="checkbox" class="m-4" name="course_name" /><span class="roboto-font">Web</span>
            &emsp;&emsp;
            <input type="checkbox" class="m-4" name="course_name" /><span class="roboto-font">DSA</span>
            <hr />
            <input type="submit" value="Apply for Admission" />
            <input type="reset" />
        </form>
    </div>
</body>
  .m-4 {
    margin: 4px;
}

input {
    background: #e4e4e4;
    line-height: 50px;
    border-radius: 5px;
    padding: 0 22px;
    font-size: 2em;
    color: #555555;
    outline: none;
    border: none;
    box-shadow: none;
    font-size: 1em;
    font-family: 'Roboto', sans-serif;
}

textarea {
    background: #e4e4e4;
    max-width: calc(100% - 52px);
    width: 100%;
    padding: 18px 22px;
    font-size: 1em;
    color: #555555;
    outline: none;
    border: none;
    box-shadow: none;
    border-radius: 5px;
    font-family: 'Roboto', sans-serif;
    resize: none;
}

select {
    line-height: 50px;
    padding: 14px 22px;
    color: #555;
    font-size: 1.2em;
    font-family: inherit;
    width: calc(50% - 10px) !important;
    border: none;
    border-radius: 5px;
}

.ubuntu-font {
    font-family: 'Ubuntu', sans-serif;
}
.roboto-font {
    font-family: 'Roboto', sans-serif;
}

h2 {
    text-align: center;
    text-transform: uppercase;
}

h4 {
    font-size: 1.4em;
    margin: 0.5em 4px;
}

h5 {
    font-size: 1em;
    text-align: right;
    display: inline-block !important;
    margin: 0.5em 4px;
    width: calc(50% - 10px) !important;
}

p {
    font-weight: 600;
    font-size: 1.1em;
    margin: 0.5em 4px;
}

.inline {
    display: inline;
    width: calc(50% - 54px);
}

body {
    background-color: #efefef;
    margin-top: 40px;
    background: linear-gradient(to top right, #88ea08 0%, #21ff90 100%);
    min-height: calc(100vh - 48px);
}

.form-container {
    padding: 15px;
    border-radius: 0px 0px 10px 10px;
    background-color: #FFFFFF;
    max-width: 50vw;
    margin: auto;
}

.title-container {
    background-color: #000000;
    padding: 20px 15px 20px;
    max-width: 50vw;
    margin: auto;
    border-radius: 10px 10px 0px 0px;
}

.title-container > h2 {
    margin: 0px;
    color: #FFFFFF;
}

hr {
    margin: 20px auto;
    border: 0; 
    border-top: 1px solid #555555;
}

input[type="submit"], input[type="reset"] {
    cursor: pointer;
    font-weight: 700;
    text-transform: uppercase;
    color: #FFFFFF;
}

input[type="submit"] {
    background-color: #82dbf7;
}
input[type="submit"]:hover {
    background-color: #269ABC;
}

input[type="reset"] {
    background: #FF4B5A;
}

input[type="reset"]:hover {
    background: #EB3746;
}

div {
    box-shadow: 0px 8px 20px 0px rgb(0 0 0 / 15%);
}
</html>
