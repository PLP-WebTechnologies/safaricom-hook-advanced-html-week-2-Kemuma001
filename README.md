1.Creating a multimedia-rich webpage with audio and video elements




     <!DOCTYPE html>
      <html lang="en">
      <head>
          <meta charset="UTF-8">
          <meta name="viewport" content="width=device-width, initial-scale=1.0">
          <title>Multimedia-Rich Webpage</title>
          <style>
             body {
               font-family: Arial, sans-serif;
               background-color: #f4f4f4;
              margin: 0;
              padding: 20px;
              text-align: center;
                     }
           audio, video {
            margin: 20px 0;
            border: 2px solid #000;
            border-radius: 10px;
                  }
            </style>
          </head>
        <body>
        <h1>Welcome to My Multimedia Webpage</h1>

    <h2>Audio</h2>
    <audio controls autoplay loop>
        <source src="audio-file.mp3" type="audio/mpeg">
        <source src="audio-file.ogg" type="audio/ogg">
        Your browser does not support the audio element.
    </audio>

     <h2>Video</h2>
    <video width="320" height="240" controls autoplay loop muted poster="poster-image.jpg">
        <source src="video-file.mp4" type="video/mp4">
        <source src="video-file.ogg" type="video/ogg">
        Your browser does not support the video tag.
    </video>
</body>
</html>






2.Designing a registration form with validation attributes




        <!DOCTYPE html>
           <html lang="en">
             <head>
                 <meta charset="UTF-8">
                 <meta name="viewport" content="width=device-width, initial-scale=1.0">
                 <title>Registration Form with Validation</title>
                                <style>
                   body {
                        font-family: Arial, sans-serif;
                        background-color: #f4f4f4;
                         display: flex;
                        justify-content: center;
                        align-items: center;
                        height: 100vh;
                        margin: 0;
                                   }
                .form-container {
                   background-color: #fff;
                   padding: 20px;
                   border-radius: 10px;
                  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
                  width: 300px;
                            }
                .form-container h2 {
                  margin-top: 0;
                 margin-bottom: 15px;
                 text-align: center;
                     }
                .form-container label {
                   display: block;
                   margin-bottom: 5px;
                        }
              .form-container input, .form-container select {
                   width: 100%;
                   padding: 10px;
                   margin-bottom: 15px;
                   border: 1px solid #ccc;
                    border-radius: 5px;
                           }
             .form-container button {
                 width: 100%;
                padding: 10px;
                background-color: #333;
               color: #fff;
               border: none;
               border-radius: 5px;
               cursor: pointer;
                       }
        .form-container button:hover {
              background-color: #555;
                  }
            </style>
         </head>
    <body>
    <div class="form-container">
        <h2>Registration Form</h2>
        <form action="#" method="post">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>

            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>

            <label for="password">Password:</label>
            <input type="password" id="password" name="password" required minlength="6">

            <label for="gender">Gender:</label>
            <select id="gender" name="gender" required>
                <option value="">Select Gender</option>
                <option value="male">Male</option>
                <option value="female">Female</option>
                <option value="other">Other</option>
            </select>

            <label for="zipcode">Zip Code:</label>
            <input type="text" id="zipcode" name="zipcode" pattern="\d{5}" required>

            <button type="submit">Register</button>
        </form>
    </div>
</body>
</html>
