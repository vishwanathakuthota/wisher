# Wisher

**Wisher** is a Python tool designed for educational purposes, simulating common techniques used in phishing and vishing. The primary goal is to provide students, educators, and security professionals with a safe, controlled way to explore these cybersecurity threats. It demonstrates how attackers craft phishing emails and vishing scenarios, highlighting the vulnerabilities in online security systems.

## ⚠️ Disclaimer

**This tool is intended solely for educational purposes.** Any unauthorized or illegal use of this tool is strictly prohibited. Always ensure you have the necessary permissions before running any simulation in a real environment. Misuse of this tool may result in serious legal consequences. The developers of this tool bear no responsibility for any damages or violations of laws incurred by improper use.

## Features

- **Phishing Simulation:** Automate the creation of fake email templates and messages for training exercises.
- **Vishing Simulation:** Use voice-based attacks for educational demonstrations, utilizing pre-recorded messages or real-time interaction.
- **Log Management:** Log all activities for further analysis and review of security breaches.

## Requirements

To run Wisher, the following dependencies are needed:

- **Python 3.x**
- **Required Packages:**
  - `requests`
  - `smtplib`
  - `flask`
  - `twilio`

You can install the necessary dependencies by running:

```bash
pip install -r requirements.txt
```

### Installation
1. Clone the Repository
```bash
git clone https://github.com/yourusername/wisher.git
cd wisher
```
2. Install Dependencies
```bash
pip install -r requirements.txt
```
Usage
-----

### Command Line Arguments

Wisher includes a variety of command-line options for simulating phishing and vishing attacks:

-   **Phishing Email Simulation**

bash

Copy code

`python wisher.py --phish --email [target_email]`

This command sends a simulated phishing email to the provided target email address.

-   **Vishing (Voice) Simulation**

To simulate a vishing attack:

bash

Copy code

`python wisher.py --vish --phone [target_phone]`


This command initiates a simulated vishing phone call to the provided number. For this feature to work, make sure you have set up your **Twilio** API credentials in the `config.py` file.

### Logging

All attack simulations are logged in the `logs/` directory. These logs can be reviewed later for understanding vulnerabilities and improving defenses.

Configuration
-------------
Before running Wisher, you'll need to configure certain settings, such as:

-   **Twilio API** (for vishing simulation)
-   **Email SMTP Server** (for phishing simulation)

Update the relevant fields in the `config.py` file.

Contributing
------------

We welcome contributions from the community. If you want to contribute:

1.  Fork the repository and give your star
2.  Create a new feature branch
3.  Make your changes and commit
4.  Open a pull request

License
-------

This project is licensed under the MIT License. See the LICENSE file for more details.
