import hashlib

def hash_password(password, algo="sha256"):
    if algo == "md5":
        return hashlib.md5(password.encode()).hexdigest()
    elif algo == "sha1":
        return hashlib.sha1(password.encode()).hexdigest()
    elif algo == "sha256":
        return hashlib.sha256(password.encode()).hexdigest()
    else:
        raise ValueError("Unsupported algorithm")

if __name__ == "__main__":
    pwd = "Password@123"
    hashed = hash_password(pwd)
    print("Password:", pwd)
    print("SHA-256 Hash:", hashed)
