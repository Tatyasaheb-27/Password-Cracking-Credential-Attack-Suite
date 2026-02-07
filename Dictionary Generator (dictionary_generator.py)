import itertools

def generate_dictionary(base_words, append_numbers=True):
    wordlist = set()

    for word in base_words:
        wordlist.add(word)
        wordlist.add(word.lower())
        wordlist.add(word.upper())
        wordlist.add(word.capitalize())

        # Leet substitutions
        leet = word.replace('a', '@').replace('s', '$').replace('o', '0')
        wordlist.add(leet)

        if append_numbers:
            for i in range(0, 100):
                wordlist.add(f"{word}{i}")

    return list(wordlist)

if __name__ == "__main__":
    base = ["admin", "password", "ganesh"]
    words = generate_dictionary(base)
    print("Sample Dictionary:", words[:10])
