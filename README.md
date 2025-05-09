# Task-2
For CodSoft intership

import random
import string

def _mix(length):
    chars = string.ascii_letters + string.digits + string.punctuation
    return ''.join(random.choice(chars) for _ in range(length))

def main():
    try:
        val = int(input("Enter a number: "))  # masked prompt
        if val < 4:
            print("Too small, try a bigger number.")
        else:
            result = _mix(val)
            print("Result:", result)  # masked output
    except Exception as e:
        print("Only numbers are allowed.")

if __name__ == "__main__":
    main()

