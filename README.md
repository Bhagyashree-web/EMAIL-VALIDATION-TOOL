


import re

def validate_email(email):
    
    email_regex = r"^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$"
    return bool(re.match(email_regex, email))

def main():
    email = input("Enter an email address: ")
    if validate_email(email):
        print("Email is valid.")
    else:
        print("Email is not valid.")

if __name__ == "__main__":
    main()

