from IPython.display import display, HTML

# Enhanced HTML structure for the newsletter with improved aesthetics
newsletter_html = """
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&family=Montserrat:wght@700&display=swap');

        /* General Styling */
        body {
            font-family: 'Roboto', sans-serif;
            color: #333;
            background-color: #f0f4f8;
            padding: 10px;
            margin: 0;
            background-image: url('https://img.freepik.com/free-vector/geometric-background-colorful-gradient_677411-3451.jpg?size=626&ext=jpg&ga=GA1.1.87617221.1726150153&semt=ais_hybrid');
            background-repeat: no-repeat;
            background-size: cover;
        }
        .container {
            margin: 0 auto;
            padding: 20px;
            background-color: white;
            border-radius: 12px;
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.1);
            max-width: 900px;
            border: 10px solid transparent;
            background-clip: padding-box;
            border-image: url('https://img.freepik.com/free-vector/geometric-background-colorful-gradient_677411-3451.jpg?size=626&ext=jpg&ga=GA1.1.87617221.1726150153&semt=ais_hybrid') 30;
        }
        .header {
            text-align: center;
            background-image: linear-gradient(rgba(0, 71, 171, 0.6), rgba(0, 71, 171, 0.6)), url('https://billing.christianacare.org/themes/cchstransparency/images/footer-logo.png');
            background-size: cover;
            background-position: center;
            padding: 40px;
            border-radius: 8px;
        }
        .title {
            font-family: 'Montserrat', sans-serif;
            font-size: 36px;
            color: #fff;
            font-weight: bold;
            text-align: center;
            letter-spacing: 2px;
            margin-bottom: 10px;
            text-transform: uppercase;
            text-shadow: 1px 1px 4px rgba(0, 0, 0, 0.4);
        }
        .subheading {
            font-style: italic;
            color: #e6f7ff;
            text-align: center;
            font-size: 20px;
            margin-bottom: 5px;
        }
        .date {
            font-size: 18px;
            color: #e6f7ff;
            text-align: center;
        }
        .section {
            margin-bottom: 40px;
            padding-bottom: 20px;
            border-bottom: 1px solid #ddd; /* Section divider */
        }
        h2 {
            color: #004080;
            font-size: 24px;
            margin-top: 20px;
            font-weight: bold;
            text-transform: uppercase;
            border-bottom: 2px solid #004080;
            padding-bottom: 5px;
        }
        p {
            font-size: 16px;
            line-height: 1.8;
            color: #333;
        }
        a {
            color: #004080;
            text-decoration: none;
            font-weight: bold;
        }
        a:hover {
            text-decoration: underline;
        }
        ul {
            list-style-type: none;
            padding: 0;
        }
        ul li {
            font-size: 18px;
            margin-bottom: 8px;
        }
        .section img {
            width: 45%; /* Consistent image size */
            height: auto;
            border-radius: 12px;
            margin-top: 15px;
            display: block;
            margin-left: auto;
            margin-right: auto;
        }

        /* Fun & Vibrant Submit Button */
        .submit-button {
            display: inline-block;
            background-color: #ff6600;
            color: white;
            padding: 12px 24px;
            font-size: 16px;
            font-weight: bold;
            border-radius: 8px;
            text-align: center;
            text-decoration: none;
            transition: background-color 0.3s ease;
        }
        .submit-button:hover {
            background-color: #e65c00;
        }

        /* Mobile Adjustments */
        @media only screen and (max-width: 600px) {
            .container {
                padding: 10px;
                max-width: 100%;
                border: none;
            }
            .title {
                font-size: 28px;
            }
            .subheading, .date {
                font-size: 16px;
            }
            .section img {
                width: 100%;
            }
            h2 {
                font-size: 20px;
            }
            ul li {
                font-size: 16px;
            }
            p {
                font-size: 14px;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <div class="title">CMIO Team Monthly IT Newsletter</div>
            <div class="subheading">Bringing the Latest IT Updates, News, and Tips to Our Healthcare Providers</div>
            <div class="date">September '24</div>
        </div>

        <!-- Table of Contents Section -->
        <div class="section">
            <h2>In this Issue:</h2>
            <ul>
                <li>Introducing DAX AI Copilot</li>
                <li>Tips & Tricks: Using Vocera Effectively</li>
                <li>PowerChart Touch Mobile App</li>
                <li>Quick IT Incident Submission</li>
                <li>Submit Your Ideas to Improve IT!</li>
            </ul>
        </div>

        <div class="section">
            <h2>Introducing DAX AI Copilot</h2>
            <p>We’re excited to introduce DAX AI Copilot, an AI tool that automates documentation during patient encounters. It listens in real-time, allowing you to focus on patient care while transcribing conversations and entering info into the EMR.</p>
            <p><b>How It Works:</b> DAX listens to the patient-provider interaction and captures key data like symptoms, diagnosis, and treatment plans to ensure accurate and timely documentation.</p>
            <p><b>Integration:</b> DAX will be integrated into the PowerMic Mobile app. If you already have the app, no need to download anything new. For those without it, instructions for setup will be shared soon.</p>
            <p><b>Timeline:</b> Our CMIO team is piloting DAX—stay tuned! Providers will attend training in October.</p>
            <img src="https://hitconsultant.net/wp-content/uploads/2023/09/IMG_2729-1500x799.png" alt="DAX AI Copilot Image">
        </div>

        <div class="section">
            <h2>Tips & Tricks: Contacting Staff via Vocera</h2>
            <p>Did you know you can reach staff on Vocera, even if you don’t know their name? Here’s how:</p>
            <p><b>Using Vocera Directory:</b> Open the directory via Vocera or hospital communication system.</p>
            <p><b>Contacting a Nurse:</b> Dial 6222, then say “nurse 6E 15 bed A” (or without the bed number). You can also use “6E RN.”</p>
            <p><b>For Those Outside the Hospital:</b> Dial 302-733-6222 and follow the same steps for room/role-based contact.</p>
            <p><b>Shortcut:</b> Use the dot phrase .nurse_for_patient for quick access.</p>
        </div>

        <!-- Quick IT Incident Submission Section -->
        <div class="section">
            <h2>Quick IT Incident Submission</h2>
            <img src="https://i.ibb.co/DVV9jtK/IT-incident-sumbission.png" alt="Quick IT Incident Submission Icon" style="width:58px; height:85px; display:block; margin:auto;">
            <p>Reporting computer or application issues is easier than ever with the Quick IT Incident Submission tool. No need to call or wait—submit problems in a few clicks.</p>
            <img src="https://i.ibb.co/8DKWXHB/it-incident.png" alt="IT Incident Submission" style="width:250px; height:200px; display:block; margin:auto;">
    
            <ul>
                <li><b>Find the Icon:</b> Look for the Quick IT Submission icon on your desktop.</li>
                <li><b>Choose Your Issue:</b> Select whether it’s a physical or application problem.</li>
                <li><b>No Contact Option:</b> If you prefer, check the option to let IT fix the issue without contacting you.</li>
                <li>Stay tuned for more updates and tips!</li>
            </ul>
        </div>

        <!-- Fun and Vibrant Submit Your Ideas Section -->
        <div class="section fun-section">
            <h2>Submit Your Ideas!</h2>
            <p>We want to hear from you! If you have ideas, suggestions, or feedback about how to improve our IT systems or processes, send them to <a href="mailto:ProviderITsuggestionbox@christianacare.org">ProviderITsuggestionbox@christianacare.org</a>.</p>
        </div>
    </div>
</body>
</html>
"""

# Display the HTML content for review
display(HTML(newsletter_html))
