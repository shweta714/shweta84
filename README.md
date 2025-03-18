//BEEPTECH
//BEEPTECH , is a health tracker customised for daily health needs of our senior citizen .It will handle their a to z health requirements starting from as basic as their step count to scheduling their appointments with doctors.


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Health Tracker</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#" class="lang-btn">English</a></li>
                <li><a href="#" class="lang-btn">Spanish</a></li>
                <li><a href="#" class="lang-btn">French</a></li>
            </ul>
        </nav>
    </header>
    
    <main>
        <div class="container">
            <section class="tracker-section">
                <h2>Step Count: <span id="step-count">0</span></h2>
                <h2>Water Intake: <span id="water-intake">0</span> mL</h2>
            </section>

            <section class="medicine-section">
                <h2>Medicine Intake</h2>
                <form>
                    <input type="text" id="medicine-name" placeholder="Medicine Name">
                    <input type="time" id="medicine-time" placeholder="Time">
                    <button type="button" id="set-medicine-btn">Set Reminder</button>
                </form>
            </section>

            <section class="appointment-section">
                <h2>Doctor's Appointment</h2>
                <form>
                    <input type="date" id="appointment-date">
                    <input type="time" id="appointment-time">
                    <button type="button" id="set-appointment-btn">Set Reminder</button>
                </form>
            </section>
        </div>

        <!-- Feedback Button -->
        <button id="open-feedback-btn">Give Feedback</button>

        <!-- Feedback Modal (Initially Hidden) -->
        <div id="feedback-modal" class="feedback-modal" style="display: none;">
            <div class="feedback-container">
                <button class="close-btn" onclick="closePopup()">❌</button>
                
                <h2>Give feedback</h2>
                <p>What do you think of Beeptech?</p>

                <!-- Emoji rating -->
                <div class="emoji-rating">
                    <span class="emoji" data-value="1">😠</span>
                    <span class="emoji" data-value="2">🙁</span>
                    <span class="emoji" data-value="3">😐</span>
                    <span class="emoji selected" data-value="4">🙂</span>
                    <span class="emoji" data-value="5">😀</span>
                </div>

                <!-- Feedback input -->
                <textarea placeholder="Do you have any thoughts you’d like to share?"></textarea>

                <!-- Follow-up question -->
                <p>May we follow up on your feedback?</p>
                <div class="follow-up">
                    <label><input type="radio" name="follow-up" value="yes" checked> Yes</label>
                    <label><input type="radio" name="follow-up" value="no"> No</label>
                </div>

                <!-- Buttons -->
                <div class="buttons">
                    <button class="send-btn">Send</button>
                    <button class="cancel-btn" onclick="closePopup()">Cancel</button>
                </div>
            </div>
        </div>

    </main>

    
</body>
</html>



 
 

