# Secure Note

A simple, browser-based encrypted note-taking application that allows you to securely store and manage your sensitive information.

## Features

- **Client-side Encryption**: All encryption/decryption happens in your browser using AES encryption
- **Password Protection**: Each note is protected with a password only you know
- **Local Storage**: Notes are saved in your browser's local storage
- **Export/Import**: Export your encrypted notes as a JSON file and import them later
- **Mobile Friendly**: Responsive design works well on all devices
- **No Server Communication**: Your data never leaves your device

## Security Details

- Uses the CryptoJS library for AES encryption
- Passwords are hashed using SHA-256 before being stored
- Only encrypted content is saved in storage
- No plaintext is ever stored or transmitted

## How to Use

### Creating and Encrypting a Note

1. Enter a title for your note
2. Write your note content in the textarea
3. Enter a strong password
4. Click "Encrypt Note" to encrypt the content
5. Click "Save Note" to save the encrypted note

### Viewing a Saved Note

1. Click "Load Notes" to see your saved notes
2. Click on a note title to load it
3. Enter the password you used to encrypt it
4. Click "Decrypt Note" to view the content

### Backing Up Your Notes

1. Click "Export Notes" to download a JSON file containing all your encrypted notes
2. Store this file securely as a backup
3. Use "Import Notes" to restore your notes from the backup file

## Privacy

This application is designed with privacy in mind:
- All processing happens locally in your browser
- No data is sent to any server
- Your notes remain private and secure

## Installation

Simply open the `secure-note.html` file in any modern web browser. No installation or server setup required.

## Technical Details

- Built with vanilla JavaScript, HTML, and CSS
- Uses the [CryptoJS](https://github.com/brix/crypto-js) library for encryption
- Notes are stored in the browser's localStorage
- Imported from CDN: `https://cdnjs.cloudflare.com/ajax/libs/crypto-js/4.1.1/crypto-js.min.js`

## License

This project is open-source and available for personal and commercial use.