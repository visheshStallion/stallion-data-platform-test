# Stallion Automotive — secure report host

This repository holds **one encrypted file** and nothing else.

`r/q7f4/index.html` is the Stallion Automotive performance dashboard, encrypted
with AES-256-GCM (PBKDF2-SHA256, 250,000 iterations). Without the passphrase it
is base64 noise — which is why it is safe to host publicly. Opening the page
asks for the passphrase and decrypts entirely in the browser; nothing is sent
anywhere.

No source code, no spreadsheets, no warehouse, no plaintext. Those live in the
private repository and never leave it. Every publish runs a leak check that
aborts if any identifying word appears in the readable part of the file.

The passphrase is not in this repository and never will be.
