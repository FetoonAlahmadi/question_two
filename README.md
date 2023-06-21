<!DOCTYPE html>
<html>
<head>
    <title>Sign Up Form Example</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f2f2f2;
            margin: 0;
            padding: 20px;
        }
        
        form {
            background-color: #fff;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 0 5px rgba(0, 0, 0, 0.1);
            width: 400px;
            margin: 0 auto;
        }
        
        h2 {
            text-align: center;
            color: #003366;
        }
        
        label {
            display: block;
            margin-bottom: 8px;
            font-weight: bold;
            color: #336699;
        }
        
        input[type="text"] {
            width: 100%;
            padding: 8px;
            border-radius: 4px;
            border: 1px solid #ccc;
        }
        
        button[type="submit"] {
            padding: 8px 16px;
            border-radius: 4px;
            background-color: #4caf50;
            color: #fff;
            border: none;
            cursor: pointer;
            margin-top: 10px;
        }
        
        button[type="submit"]:hover {
            background-color: #45a049;
        }
        
        #output {
            margin-top: 20px;
            font-weight: bold;
            color: #336699;
            text-align: center;
        }
    </style>
    <script>
        function handleSubmit() {
            // Handle form submission logic here
            // You can access form data using JavaScript and perform any desired actions
            
            // Example: Display a message
            var firstName = document.getElementById('firstName').value;
            var lastName = document.getElementById('lastName').value;
            var message = "Congratulations " + firstName + " " + lastName + ", you are now signed up.";
            document.getElementById('output').innerHTML = message;
            
            // Prevent form submission
            return false;
        }
    </script>
</head>
<body>
    <form onsubmit="return handleSubmit()">
        <h2>Sign Up Form Example</h2>
        
        <label for="firstName">First , Last Name*:</label>
        <input type="text" id="firstName" name="firstName" placeholder="Type your first Name here" required>  <input type="text" id="lastName"  placeholder="Type your last Name here" name="lastName" required><br>
		
        
        <label for="Organization">Organization:</label>
        <input type="text" id="Organization" name="Organization">
        
        <label for="Email address">Email address*:</label>
        <input type="text" id="Email address" placeholder="name@domain.com" name="Email address" required>
        
        <label for="Work Phone">Work Phone:</label>
        <input type="text" id="Work Phone" name="Work Phone">
        
        <label for="Home Phone">Home Phone:</label>
        <input type="text" id="Home Phone" name="Home Phone">
        
        <label for="Cell Phone">Cell Phone:</label>
        <input type="text" id="Cell Phone" name="Cell Phone">
        
        <label for="Fax">Fax:</label>
        <input type="text" id="Fax" name="Fax">
        
        <label for="Address1">Address1*:</label>
        <input type="text" id="Address1" name="Address1" placeholder="Type your Address1 here" required>
        
        <label for="Address2">Address2:</label>
        <input type="text" id="Address2" name="Address2">
        
        <label for="City">City*:</label>
        <input type="text" id="City" placeholder="Type your City here" name="City" required>
        
        <label for="State">State:</label>
        <input type="text" id="State" name="State">
        
        <label for="Zip Postal Code">Zip Postal Code:</label>
        <input type="text" id="Zip Postal Code" name="Zip Postal Code">
        
        <label for="Country">Country*:</label>
        <input type="text" id="Country" placeholder="Type your Country here" name="Country" required>
        
        <label for="required field">Required field*:</label>
        
        <button type="submit">Submit</button>
        <a href="file:///C:/Users/me/OneDrive/%D8%B3%D8%B7%D8%AD%20%D8%A7%D9%84%D9%85%D9%83%D8%AA%D8%A8/project/formtest.html">Form</a>
    </form>

    <div id="output"></div>
</body>
</html>
