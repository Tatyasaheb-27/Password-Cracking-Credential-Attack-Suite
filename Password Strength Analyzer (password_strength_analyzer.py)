import math
import string

def calculate_entropy(password):
    charset = 0
    if any(c.islower() for c in password): charset += 26
    if any(c.isupper() for c in password): charset += 26
    if any(c.isdigit() for c in password): charset += 10
    if any(c in string.punctuation for c in password): charset += 32

    return len(password) * math.log2(charset) if charset else 0

def analyze_password(password):
    entropy = calculate_entropy(password)

    strength = "Weak"
    if entropy > 60:
        strength = "Strong"
    elif entropy > 40:
        strength = "Moderate"

    return {
        "password": password,
        "length": len(password),
        "entropy": round(entropy, 2),
        "strength": strength
    }

if __name__ == "__main__":
    result = analyze_password("Password@123")
    print(result)
