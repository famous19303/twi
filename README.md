[![Pylint](https://github.com/RAHB-REALTORS-Association/sms-sender/actions/workflows/pylint.yml/badge.svg?branch=master)](https://github.com/RAHB-REALTORS-Association/sms-sender/actions/workflows/pylint.yml)[![Python 3.9](https://github.com/RAHB-REALTORS-Association/sms-sender/actions/workflows/python-3.9.yml/badge.svg?branch=master)](https://github.com/RAHB-REALTORS-Association/sms-sender/actions/workflows/python-3.9.yml)[![Python 3.10](https://github.com/RAHB-REALTORS-Association/sms-sender/actions/workflows/python-3.10.yml/badge.svg?branch=master)](https://github.com/RAHB-REALTORS-Association/sms-sender/actions/workflows/python-3.10.yml)[![Python 3.11](https://github.com/RAHB-REALTORS-Association/sms-sender/actions/workflows/python-3.11.yml/badge.svg?branch=master)](https://github.com/RAHB-REALTORS-Association/sms-sender/actions/workflows/python-3.11.yml)

***Notice: this project is not supported or endorsed by Twilio Inc. in any way***

# Bulk SMS Sender

## About
Bulk SMS Sender is a web-based app that uses a Twilio account to send SMS messages in bulk from a CSV file.

## Usage
The user saves the data on a CSV file with 3 columns and use a webform to update the CSV file with their Twilio credentials. The backend uses
Twilio's Python SDK to send the messages and generate a delivery report.

## Tech stack
- Python 3.9 - 3.11
- Flask 2.2+
- GUnicorn 20.1+
- Twilio Python Libraries 7.14+

## Deploying

[![Deploy to DO](https://www.deploytodo.com/do-btn-blue.svg)](https://cloud.digitalocean.com/apps/new?repo=https://github.com/RAHB-REALTORS-Association/sms-sender/tree/master)

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/RAHB-REALTORS-Association/sms-sender/tree/master)

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/RAHB-REALTORS-Association/sms-sender/tree/master)

Review settings.py before deployment, especially the following settings:
- Line 2: Testing
- Line 3: Flask secret. Generate a random Secret on deployment
- Line 6: Set the upload folder according to your OS
