# Password Strength Analyzer

A modern, interactive web-based password strength checker that evaluates your password in real-time and provides suggestions for creating stronger passwords.

## Features

- **Real-time Strength Analysis**: Instantly see your password strength as you type
- **Visual Strength Meter**: Dynamic progress bar that fills based on password strength (0-100)
- **Detailed Weakness Detection**: Get specific feedback on what makes your password weak
- **Smart Password Suggestions**: Automatically generates strong password suggestions when your current password scores below 70%
- **Character Variety Requirements**: Checks for uppercase, lowercase, numbers, and special characters

## Password Strength Criteria

The analyzer evaluates your password based on the following criteria:

### Length Requirements
- **5 characters or less**: Too short (-40 points)
- **6-10 characters**: Could be longer (-15 points)
- **11+ characters**: Good length (no deduction)

### Character Variety
- **Uppercase letters**: Missing (-20 points), Less than 2 (-5 points)
- **Lowercase letters**: Missing (-20 points), Less than 2 (-5 points)
- **Numbers**: Missing (-20 points), Less than 2 (-5 points)
- **Special characters**: Missing (-20 points), Less than 2 (-5 points)

### Common Issues
- **Repeated characters**: Each occurrence deducts 10 points (e.g., "aaa" = -20 points)
- **Common passwords**: Passwords like "password", "123456", "qwerty", "admin", "password123" result in -40 points

## How to Use

1. Open `password.html` in your web browser
2. Type your password in the input field
3. Watch the strength meter fill based on your password strength
4. Review the weakness messages below the input field
5. See suggested strong passwords when your current password scores below 70%

## Scoring System

- **0-30**: Very Weak (Red)
- **30-60**: Weak (Orange)
- **60-75**: Fair (Yellow)
- **75-90**: Strong (Light Green)
- **90-100**: Very Strong (Green)

## Tips for Creating Strong Passwords

✓ **Use at least 12 characters** - The longer, the better  
✓ **Mix uppercase and lowercase letters** - Vary the case throughout  
✓ **Include numbers** - Use multiple numbers, not just at the end  
✓ **Add special characters** - Use symbols like !@#$%^&*()_+  
✓ **Avoid common patterns** - Don't use dictionary words or keyboard patterns  
✓ **Don't repeat characters** - Avoid "aaa" or "111" patterns  
✓ **Make it unique** - Use different passwords for different accounts  

## Example Strong Passwords

The analyzer generates suggestions like:
- `K9@mL2$xQ!pR5vN`
- `B4#nP8$jT!sH6cM`
- `D7*fG3@wE5!rY9q`

## Browser Compatibility

Works on all modern browsers that support:
- HTML5
- CSS3 (Flexbox, Gradients, CSS Variables)
- ES6 JavaScript

## Installation

Simply download `password.html` and open it in any modern web browser. No server or dependencies required!

## Code Structure

- **HTML**: Simple semantic structure with input field and display elements
- **CSS**: Modern gradient design with smooth animations and responsive layout
- **JavaScript**: Real-time password analysis with multiple weakness detection functions

### Key JavaScript Functions

- `updateStrengthMeter()`: Main function that recalculates strength on input
- `calculatePasswordStrength()`: Evaluates all weakness criteria
- `generateStrongPassword()`: Creates a random strong password suggestion
- `characterTypeWeakness()`: Checks for required character types

## Future Enhancements

- Export password strength statistics
- Password history tracking
- Keyboard pattern detection
- Pronunciation-friendly password generation
- Dark/Light mode toggle
- Multi-language support

## License

Open source - Feel free to use and modify as needed!

---

**Note**: Never share your passwords with anyone, and avoid entering real passwords into untrusted websites. This tool runs entirely in your browser with no data transmission to external servers.
