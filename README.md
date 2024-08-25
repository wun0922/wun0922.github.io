<!DOCTYPE html>

<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Instagram Tracker</title>

</head>

<body>

    <h1>Instagram Tracker</h1>

    <form id="login-form">

        <label for="username">Username:</label>

        <input type="text" id="username" name="username" required><br><br>

        

        <label for="password">Password:</label>

        <input type="password" id="password" name="password" required><br><br>

        

        <button type="submit">Login</button>

    </form>



    <div id="tracker-section" style="display:none;">

        <h2>Welcome, <span id="user-display"></span></h2>

        <button id="track-followers">Track Followers</button>

        <button id="track-followings">Track Followings</button>

        <button id="track-unfollowers">Track Unfollowers</button>

        

        <div id="results"></div>

    </div>



    <script>

        // Example JavaScript for handling form submission

        document.getElementById('login-form').addEventListener('submit', function(e) {

            e.preventDefault();

            const username = document.getElementById('username').value;

            const password = document.getElementById('password').value;



            // Normally, you'd send this to a secure server

            console.log('Login attempt with', username, password);



            // Mock successful login

            document.getElementById('user-display').innerText = username;

            document.getElementById('tracker-section').style.display = 'block';

        });



        // Example functions for tracking (would require real backend implementation)

        document.getElementById('track-followers').addEventListener('click', function() {

            document.getElementById('results').innerText = 'Tracking Followers...';

        });



        document.getElementById('track-followings').addEventListener('click', function() {

            document.getElementById('results').innerText = 'Tracking Followings...';

        });



        document.getElementById('track-unfollowers').addEventListener('click', function() {

            document.getElementById('results').innerText = 'Tracking Unfollowers...';

        });

    </script>

</body>

</html>
