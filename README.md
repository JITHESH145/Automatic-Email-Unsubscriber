# Email Unsubscriber

## Overview
This script connects to a Gmail inbox, searches for emails containing the word "unsubscribe," extracts unsubscribe links from the email body, and attempts to visit them automatically. It also saves the extracted links to a text file.

## Features
- Connects securely to a Gmail inbox using IMAP.
- Searches for emails containing the word "unsubscribe."
- Extracts unsubscribe links from email HTML content.
- Visits the unsubscribe links automatically.
- Saves extracted links to a text file (`links.txt`).

## Prerequisites
Ensure you have the following installed:
- Python 3.x
- Required Python libraries:
  - `imaplib`
  - `email`
  - `os`
  - `dotenv`
  - `bs4` (BeautifulSoup)
  - `requests`

## Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/JITHESH145/Automatic-Email-Unsubscriber
   cd repository-name
   ```
2. Install the required dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Create a `.env` file and add your email credentials:
   ```sh
   EMAIL=your-email@gmail.com
   PASSWORD=your-email-password
   ```
   **Note:** Using app-specific passwords instead of your actual password is recommended for security.

## Usage
Run the script:
```sh
python script.py
```

## How It Works
1. Logs into your Gmail inbox using IMAP.
2. Searches for emails that contain the word "unsubscribe."
3. Extracts unsubscribe links from the email content.
4. Visits each extracted link to attempt automatic unsubscription.
5. Saves all found links to `links.txt`.

## Security Considerations
- Store sensitive credentials in a `.env` file and **never** share it.
- Consider using OAuth for secure authentication instead of plain text credentials.
- Be cautious while automatically clicking unsubscribe links, as some may be malicious.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing
Feel free to fork this repository, open issues, or submit pull requests to enhance functionality.

## Disclaimer
Use this script responsibly. Automating unsubscribe actions may not always work and could have unintended consequences.

