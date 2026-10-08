# Advanced Password Strength Checker

A simple but advanced password strength checker built with Python and Tkinter.

It checks a password in real time and gives a strength score based on length, character types, entropy, common passwords, patterns, and other basic security checks.

## Features

- Real-time password strength checking
- Security score out of 10
- Password entropy calculation
- Uppercase and lowercase detection
- Number detection
- Special character detection
- Password length checking
- Common password detection
- Common pattern detection
- Repeated character detection
- Estimated brute-force resistance
- Visual strength meter
- Show/hide password
- Dark-themed GUI
- Works completely locally
- Can be converted into a Windows `.exe`

## Screenshot

Add the screenshot here:

```text
screenshots/password-checker.png
```

Then use:

```markdown
![Password Strength Checker](screenshots/password-checker.png)
```

## Technologies

- Python
- Tkinter
- Regular Expressions
- Math
- PyInstaller

No external Python packages are required to run the application.

## Project Structure

```text
advanced-password-strength-checker/
│
├── Password.py
├── README.md
├── requirements.txt
├── LICENSE
├── .gitignore
│
└── screenshots/
    └── password-checker.png
```

The Windows `.exe` can be uploaded separately through GitHub Releases.

## How to Run

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/advanced-password-strength-checker.git
```

Go to the project folder:

```bash
cd advanced-password-strength-checker
```

Run the program:

```bash
python Password.py
```

## Create Windows EXE

Install PyInstaller:

```bash
pip install pyinstaller
```

Build the application:

```bash
pyinstaller --onefile --windowed --name "Password Strength Checker" Password.py
```

The executable will be available in:

```text
dist/
└── Password Strength Checker.exe
```

The `.exe` can then be shared with other Windows computers without requiring Python to be installed.

## How It Works

The program checks several properties of the password.

### Password Length

Longer passwords generally provide a larger search space.

The application checks for passwords with:

```text
12+ characters
16+ characters
```

### Character Types

The program checks whether the password contains:

```text
Uppercase letters
Lowercase letters
Numbers
Special characters
```

Example:

```text
CyberSecurity@2026
```

### Entropy

The program estimates password entropy based on the password length and possible character pool.

Higher entropy generally means a larger theoretical search space.

### Common Password Detection

The program checks for commonly used passwords such as:

```text
password
123456
qwerty
admin
password123
```

### Pattern Detection

It also looks for simple patterns such as:

```text
123
abcd
qwerty
password
```

### Repeated Characters

Simple repeated patterns such as:

```text
aaa
111
!!!
```

are treated as weak characteristics.

## Strength Levels

The application gives the password one of these levels:

| Level | Description |
|---|---|
| VERY WEAK | Easily guessable |
| WEAK | Low complexity |
| MODERATE | Reasonable but can be improved |
| STRONG | Good complexity |
| VERY STRONG | High complexity and entropy |

## Privacy

The password is analyzed locally on the computer.

The application does not intentionally:

- Upload passwords
- Store passwords
- Send passwords to a server
- Save passwords in a database

The application can work without an internet connection.

Still, don't enter real passwords into software you don't trust.

## Limitations

This is an educational password-strength checker.

The entropy and brute-force estimates are theoretical estimates. They don't guarantee that a password will take a particular amount of time to crack.

Real-world security also depends on:

- Password hashing
- Hashing algorithm
- Attacker hardware
- Rate limiting
- Multi-factor authentication
- Password reuse
- Data breaches
- Authentication system design

A password can appear strong but still be unsafe if it has already been exposed in a data breach.

## Cybersecurity Concepts

This project helped me work with:

- Password security
- Authentication
- Password entropy
- Brute-force attacks
- Dictionary attacks
- Pattern detection
- Input validation
- Regular expressions
- Python GUI development
- Basic security tool development

## Future Improvements

Some things I may add later:

- Secure password generator
- Larger password dictionary
- Breached-password detection
- Keyboard pattern detection
- Name and date pattern detection
- Unit tests
- Better entropy analysis
- Custom application icon
- Automated GitHub builds
- Cross-platform support

## Author

Amarnadh

BCA Cybersecurity Student

Interested in cybersecurity, ethical hacking, network security and security tool development.

## License

This project is licensed under the MIT License.

See the `LICENSE` file for more information.
