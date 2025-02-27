﻿# BokoHacks 2025
An overview of the hackathon project made by Kayla Vincent, Makenna Wilson, and Brittany Hale for Texas State University's 2025 BokoHacks hackathon!
# Tools and Resources
A free version of ChatGPT was utilized for debugging help and supplementing information about Flask, Python, and SQL syntaxes. Websites like GeeksForGeeks and Stack Overflow were used to problem-solve and brainstorm solutions to the included vulnerabilities. Additional tools include the Python library bleach, which had to be imported for input sanitization. Python, SQLite, Flask, and VS Code were used to develop this program.
# Requirements
- Python 3.8 or higher → <a href="https://www.python.org/downloads/">Download Python</a>
- Pip (Python package installer)
- SQLite → <a href="https://www.sqlite.org/download.html">Download SQLite</a> (Optional if you want binaries otherwise; dependencies should install automatically)
- Modern web browser (Chrome/Firefox recommended)
- Text editor or IDE VS Code recommended → <a href="https://code.visualstudio.com/docs/python/environments">VS Code Setup</a>
# Setup Instructions
1. Clone the repository:

2. Set up git and create virutal environment
3. Install dependencies:
pip install -r requirements.txt
pip install bleach
4. Start the application:
python app.py
5. Open <a href="http://localhost:5000/">http://localhost:5000/</a> in your browser
# Testing Guide
The following processes should be done in order to test the new security implementations for the website:
- Creating a new user: shows update made to Captcha generation.
- Creating a new note: in the section labeled "Sample Test Inputs" at the bottom of the page, there is an area dedicated to test inputs for notes creation. This is to make your life easier! Feel free to use any other test input to see the newest notes functionality.
# Future Improvements
- Add multi-factor authentication using an email the user inputs when they first create their account. We have an idea for how this could be implemented, but due to timing restrictions we did not include this in the final program.
- Use HTTPS instead of HTTP. If this site were to be published, rather than just run off of the localhost, a certificate could be obtained to upgrade the site from HTTP to HTTPS.
- The upgrade to HTTPS would also allow the successful integration of VirusTotal into the code. VirusTotal would scan uploaded files for malicious content and delete them if any malware is found inside. However, the HTTP protocol causes files to automatically be flagged as "insecure" and deletes them regardless of the file's content.
- Change formatting for News images so that they fit into the display window
# Sample Test Inputs
User Creation:
Example Passwords:
goodInput12345@#
badpassword

Notes Creation:
Example Title (tests max char length of 150): &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&

Example Content I (tests bleaching): 
"<script>alert('This is a bad script!');</script>"
"<p>This is a <strong>safe</strong> paragraph.</p>"

Example Content II (tests max char length of 2000):
&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&
