# python-assignment-2
def create_char_frequency_dict(string):
    frequency_dict = {}
    for char in string:
        if char in frequency_dict:
            frequency_dict[char] += 1
        else:
            frequency_dict[char] = 1
    return frequency_dict

def print_histogram(frequency_dict):
    print("Character Frequency Histogram:")
    for char, frequency in frequency_dict.items():
        print(char, "-" * frequency)

def main():
    user_input = input("Enter a string: ")
    frequency_dict = create_char_frequency_dict(user_input)
    print_histogram(frequency_dict)

if __name__ == "__main__":
    main()
