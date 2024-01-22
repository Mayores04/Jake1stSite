
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Demographic Information</title>
    <!-- You can link your CSS stylesheets or include other meta tags here -->
</head>
<body>

    <header>
        <h1>Profile: </h1>
    </header>

    <nav>
        <!-- You can add navigation links here -->
    </nav>

    <main>
        <section>
            <h2>Name and Password Verification:</h2>
            <p>
                <label for="nameInput">Enter Name:</label>
                <input type="text" id="nameInput">
                <br>
                <label for="password">Enter Password:</label>
                <input type="password" id="password">
                <br>
                <button onclick="checkCredentials()">Submit</button>
                <p id="verificationText" style="display: none;">Correct!!!</p>

                <script>
                    function checkCredentials() {
                        const nameInput = document.getElementById('nameInput');
                        const passwordInput = document.getElementById('password');
                        const verificationText = document.getElementById('verificationText');

                        const enteredName = nameInput.value.trim().toUpperCase();
                        const enteredPassword = passwordInput.value;

                        // Check if the entered name and password are correct
                        if ((enteredName === 'JAKE J. MAYORES' || enteredName === 'Angelika Bianca L. Upao') && (enteredPassword === 'J@k3m@y0res' || enteredPassword === 'Angelika30')) {
                            verificationText.style.display = 'block';
                        } else {
                            alert('Please enter the correct name and password.');
                        }
                    }
                </script>
            </p>
        </section>

        <section>
            <h1>EMAIL ACCOUNT</h1>
            <!-- Your existing password section remains unchanged -->

            <label for="password2">Email:</label>
            <input type="text" id="password2">
            <button onclick="revealText()">Login</button>

            <p id="protectedText" style="display: none;">Email has been verified.<br>You can now access Jake Account on Face Book. <br>https://www.facebook.com/jakejmayores</p>

            <script>
                function revealText() {
                    const nameInput = document.getElementById('nameInput');
                    const passwordInput = document.getElementById('password');
                    const password2Input = document.getElementById('password2');
                    const protectedText = document.getElementById('protectedText');

                    const enteredName = nameInput.value.trim().toUpperCase();
                    const enteredPassword = passwordInput.value;
                    const enteredEmailPassword = password2Input.value;

                    // Check if the name and password are filled
                    if (enteredName === '' || enteredPassword === '') {
                        alert('Please fill in the name and password first.');
                        return;
                    }

                    // Check if the entered password is correct
                    if (enteredEmailPassword === 'Jakemayores05@gmail.com' || enteredEmailPassword === 'angelikaupao@gmail.com') {
                        protectedText.style.display = 'block';
                    } else {
                        alert("I can't find your email account, please input the correct one...");
                    }
                }
            </script>
        </section>
    </main>

    <footer>
        <p>ACCESS JAKE ACCOUNT</p>
    </footer>

</body>
</html>
