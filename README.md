# Simple Password Generator (SPG)

A lightweight, client-side password generator built with plain HTML, CSS, and JavaScript.

SPG generates passwords directly in your browser using the **Web Crypto API** for cryptographically secure random values.

## Features

* Generate passwords from **8–32 characters**
* Uppercase letters (`A-Z`)
* Lowercase letters (`a-z`)
* Numbers (`0-9`)
* Special characters (`-._#$@%!`)
* Additional symbols (`"+(){}[]?&,*<>|:;^`)
* Cryptographically secure random generation using `crypto.getRandomValues()`
* Copy generated passwords to the clipboard
* No account required
* No backend required
* No database
* No password storage
* No tracking
* Works entirely in the browser

## Privacy

SPG does **not** store generated passwords.

There is:

* No database
* No `localStorage`
* No IndexedDB
* No server-side processing
* No user accounts
* No password history

The generated password exists only in the browser while the page is open. Refreshing or closing the page removes it.

## How It Works

SPG is a completely client-side application.

The browser loads the HTML, CSS, and JavaScript, and all password generation happens locally.

Random characters are selected using the browser's Web Crypto API rather than `Math.random()`.

The generator ensures that each selected character type contributes at least one character when multiple character types are enabled, then securely shuffles the resulting password.

## Usage

1. Open SPG in a web browser.
2. Select the character types you want to use.
3. Choose the desired password length.
4. Click **Generate Password**.
5. Click **Copy** to copy the password.
6. Use the password wherever you need it.

## Technology

SPG is intentionally simple:

* HTML
* CSS
* JavaScript
* Web Crypto API

No frameworks, libraries, build system, or backend are required.

## License

SPG is licensed under the **GNU Affero General Public License v3.0 (AGPL-3.0)**.

See the **[LICENSE](https://github.com/nxs8739/spg/blob/main/LICENSE)** file for the full license text.
