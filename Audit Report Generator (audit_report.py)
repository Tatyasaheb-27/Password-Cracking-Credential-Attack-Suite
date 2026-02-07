def generate_report(results):
    print("\n--- Password Security Audit Report ---")
    for r in results:
        print(f"Password: {r['password']}")
        print(f"Length: {r['length']}")
        print(f"Entropy: {r['entropy']}")
        print(f"Strength: {r['strength']}")
        print("-" * 40)

if __name__ == "__main__":
    sample = [{
        "password": "admin123",
        "length": 8,
        "entropy": 28.5,
        "strength": "Weak"
    }]
    generate_report(sample)
