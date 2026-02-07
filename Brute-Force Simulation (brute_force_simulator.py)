import itertools
import string
import hashlib
import time

def brute_force_simulation(target_hash, max_length=4):
    charset = string.ascii_lowercase + string.digits
    start_time = time.time()

    for length in range(1, max_length + 1):
        for combo in itertools.product(charset, repeat=length):
            attempt = ''.join(combo)
            attempt_hash = hashlib.sha256(attempt.encode()).hexdigest()

            if attempt_hash == target_hash:
                return attempt, time.time() - start_time

    return None, None

if __name__ == "__main__":
    target = hashlib.sha256("test1".encode()).hexdigest()
    password, duration = brute_force_simulation(target)
    print("Cracked Password:", password)
    print("Time Taken:", round(duration, 2), "seconds")
