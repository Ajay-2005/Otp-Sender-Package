# Email OTP Sender

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![npm Version](https://img.shields.io/npm/v/email-otp-sender.svg)](https://www.npmjs.com/package/otp-email-sender)

A simple and lightweight npm package for sending one-time passwords (OTPs) via email using Nodemailer.

## Features

- Generate and send one-time passwords (OTPs) via email
- Simple and easy to use

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on GitHub.

## Installation

Install the package using npm:

```bash
npm install email-otp-sender
```

## Usage

```javascript

import sendOtpEmail from 'email-otp-sender';

const senderEmail = 'your-email@example.com';
const senderPassword = 'your-email-password';
const recipientEmail = 'recipient-email@example.com';
const subject = 'OTP Verification';

sendOtpEmail(senderEmail, senderPassword, recipientEmail, subject)
  .then((response) => {
    console.log(response);
  })
  .catch((error) => {
    console.error('Error:', error);
  });
```

Make sure to replace 

- your-email@example.com with your actual sender email
- your-email-password with the password of your sender email
- recipient-email@example.com with the recipient's email address
- OTP Verification with your desired subject.