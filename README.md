
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Baloo+Bhai+2&display=swap" rel="stylesheet">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Roboto+Condensed:wght@300&display=swap" rel="stylesheet">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Oswald:wght@200&display=swap" rel="stylesheet">
    <style>
        body {
            background: url('https://images.pexels.com/photos/261679/pexels-photo-261679.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')no-repeat center center/cover;
            display: flex;
            flex-direction: column;
        }

        div {
            font-family: 'Roboto Condensed', sans-serif;
        }

        .heading {
            display: flex;
            color: black;
            background-color: rgb(5 199 11);
            font-family: 'Oswald', sans-serif;
            padding: 20px 0px;
            margin: 0px 0px;
            margin-right: 30%;
            /* margin: 0px 72px; */
            border-radius: 5px;
        }

        h1 {
            padding-left: 8%;
            padding-right: 40%;
            font-size: 50px;
            margin: 10px;
            /* text-shadow: 2px 1px black; */
        }

        form div input {
            margin: 10px 5px;
            padding: 5px 5px;
            /* border: 2px solid black; */
            border-radius: 5px;

        }

        .name input,
        .email input,
        .e-id input,
        .dept input,
        .roll input {
            width: 90%;
            height: 25px;
            box-shadow: 3px 2px black;
        }

        form div {
            margin: 10px 5px;
            padding: 5px 5px;
            /* border: 2px solid black; */
            border-radius: 5px;
            /* background-color: #ffffff14; */
            font-weight: bolder;
        }

        .exceptsubmit div:hover {
            background-color: #ffffff52;
        }

        .container {
            display: flex;
            flex-direction: column;
            background-color: rgba(240, 248, 255, 0);
            margin-left: 6%;
        }

        .container {
            width: 70%;
        }

        /* .container div div{
            width: 55%;
        } */

        input {
            font-size: 15px;
        }

        body::before {
            background: url('https://images.pexels.com/photos/261679/pexels-photo-261679.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1')no-repeat center center/cover;
            content: "";
            opacity: 0.1;
        }

        .gender input {
            margin: 8px;
        }

        .submit input {
            background-color: #b9b1ff;
            font-size: 15px;
            color: #001ff9;
            font-family: 'Baloo Bhai 2', cursive;
            cursor: pointer;
            padding: 3px 10px;
            border-radius: 3px;
            transition: all 0.1s;
            box-shadow: 2px 3px black;
        }

        .submit input:hover {
            color: rgba(233, 233, 233, 0.871);
            background-color: #a6a9ffe3;
            height: 36px;
            width: 70px;
        }
        .submit button:hover{
            color: rgba(233, 233, 233, 0.871);
            background-color: #a6a9ffe3;
            height: 35px;
            width: 59px;
        }
        .submit button{
            background-color: #b9b1ff;
            font-size: 15px;
            color: #001ff9;
            font-family: 'Baloo Bhai 2', cursive;
            cursor: pointer;
            padding: 3px 10px;
            border-radius: 3px;
            transition: all 0.1s;
            box-shadow: 2px 3px black;
        }
        #designation {
            margin: 10px 5px;
            /* margin-left: 50px; */
            padding: 5px 5px;
            /* border: 2px solid black; */
            border-left: 2px solid black;
            border-top: 2px solid black;
            border-radius: 5px;
            width: 91%;
            height: 38px;
            text-align: center;
            box-shadow: 3px 2px black;
        }

        /* .heading{
            position: sticky;
            top: 0px;
        } */
        .designation {
            width: 60%;
        }

        .class {
            margin: 2px;
        }

        p {
            color: red;
        }

        @media (max-width: 500px) {
            .container div {
                width: 90%;
            }
        }

        @media (min-width: 500px) and (max-width: 875px) {
            .container div {
                width: 80%;
            }
        }

        @media (min-width: 875px) and (max-width: 1400px) {
            .container div {
                width: 70%;
            }
        }

        @media (min-width: 1400px) and (max-width: 2150px) {
            .container div {
                width: 60%;
            }
        }
    </style>
</head>

<body>
    <div class="heading">
        <h1>College Registration Form</h1>
    </div>
    <form action="" name="form1">
        <div class="container">
            <div class="exceptsubmit">
                <div class="name">
                    Name*
                    <input type="text" id="idname" name="name1" required>
                </div>
                <div class="email">
                    Email*
                    <input type="email" name="email" id="emailid" required>
                </div>
                <div class="designation">

                    Designation*
                    <select name="designation" id="designation" onchange="checkvalue(this.value);" required>
                        <option value="none">--Select --</option>
                        <option value="1">Proffesor</option>
                        <option value="2">Student</option>
                    </select>
                </div>
                <div class="gender">
                    Gender*:
                    <br>
                    <input type="radio" name="gender" value="male" required>Male
                    <input type="radio" name="gender" value="female">Female
                    <input type="radio" name="gender" value="others">Others
                </div>
                <div class="e-id" id="empid" style="display: none;">
                    Employee id*
                    <input type="text" name="empid" required>
                </div>

                <div class="roll" id="roll1" style="display: none;">
                    Roll number*
                    <input type="text" name="roll1" required>
                </div>
                <div class="dept" id="dept" style="display: none;">
                    Department
                    <input type="text">
                </div>
            </div>
            <p>* signnifies important areas to be filled</p>
            <div class="submit">
                <input type="submit" value="submit"
                    onclick="stringlengthmin(document.form1.name1,2),stringlengthmaxempid(document.form1.empid,8),stringlengthmaxrollno(document.form1.roll1,8),message()"
                    id="submit">
                <button onclick="resetmessage()" >reset</button>
            </div>
        </div>
    </form>
    <script>

        function stringlengthmin(inputtxt, minlength) {
            let field = inputtxt.value;
            let minlen = minlength;

            if (field.length <= minlen) {
                alert("Name should have atleast " + minlen + " letters");
            }
        }
        function stringlengthmaxempid(inputtxt, maxlength) {
            let field = inputtxt.value;
            let maxlen = maxlength;

            if (field.length >= maxlen) {
                alert("Employee id should have maximum " + maxlen + " characters");
            }

        }

        function stringlengthmaxrollno(inputtxt, maxlength) {
            let field = inputtxt.value;
            let maxlen = maxlength;

            if (field.length >= maxlen) {
                alert("Roll no. should have maximum " + maxlen + " characters");
            }
        }

        function checkvalue(val) {
            if (val == "1") {
                document.getElementById('empid').style.display = 'block';
                document.getElementById('roll1').style.display = 'none';
                document.getElementById('dept').style.display = 'block';
                return 1;
            }
            else if (val == "2") {
                document.getElementById('empid').style.display = 'none';
                document.getElementById('roll1').style.display = 'block';
                document.getElementById('dept').style.display = 'block';
                return 0;
            }
            // else 
            // {
            //     document.getElementById('empid').style.display = 'none';
            //     document.getElementById('roll1').style.display = 'none';
            //     document.getElementById('dept').style.display = 'none';
            // }
        }
        function ValidateEmail(inputText) {
            var mailformat = /^\w+([\.-]?\w+)*@\w+([\.-]?\w+)*(\.\w{2,3})+$/;
            if (inputText.value.match(mailformat)) {
                return 1;
            }
            else {
                return 0;
            }
        }

        function message() {
            let empidlen = document.form1.roll1.value.length;
            let rolllen = document.form1.roll1.value.length;
            let genval = document.form1.gender.value;
            let emailval = document.form1.email;
            if ((document.form1.name1.value.length >= 2) && (empidlen <= 8 && empidlen > 0) && (rolllen <= 8 && rolllen > 0) && (document.form1.designation.value == 1 || document.form1.designation.value == 2) && (genval == "male" || genval == "female" || genval == "others") && (ValidateEmail(emailval)==1))
            alert("Form is successfully submitted");
        }
        function resetmessage()
        {
            let check=confirm("Do you want to reset");
            if(check)
            form1.reset();
        }
    </script>
</body>
</html>
