# ISS Tracker + Email Notifier

The ISS Tracker and Email Notifier is a Python script that tracks the International Space Station's (ISS) location and sends an email notification when specific conditions are met. The script uses the Open Notify API to get the ISS's current position and the Sunrise Sunset API to determine sunrise and sunset times at a given location.

## Prerequisites

1. Python 3.x
2. Required libraries: `requests`, `time`, `smtplib`.

## Setup

Replace the placeholders in the script:
   - Set `MY_LAT` and `MY_LONG` to your latitude and longitude coordinates.
   - Replace `my_email` with your Gmail email address.
   - Replace `password` with your Gmail app password.
   - Modify the email details in the `connection.sendmail()` function to match your recipient's email.

## Usage

1. Run the script
   
2. The script will continuously monitor the ISS's position and time conditions.

3. If the ISS is within a certain proximity of your coordinates and it's between sunset and sunrise, the script will send an email notification.

4. Go outside and look up to possibly spot the ISS

## Notes

- Make sure your Gmail account allows less secure apps and generate an app password for the script.
- The script runs continuously until you manually stop it.
