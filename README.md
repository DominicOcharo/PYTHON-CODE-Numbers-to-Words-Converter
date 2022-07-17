# PYTHON-CODE-Numbers-to-Words-Converter
#This is a python code that converts numerical numbers to words

class NumbersConverter:

    def __init__(self, numbers):
        self.no = numbers

    def numbers_to_words(self):
        numb_dict = {
            "1": "one",
            "2": "two",
            "3": "three",
            "4": "four",
            "5": "five",
            "6": "six",
            "7": "seven",
            "8": "eight",
            "9": "nine",
            "0": "zero"
        }
        output = ''
        for characters in self.no:
            output += numb_dict.get(characters, characters) + ' '
        print(output)


numbers = input("Input numbers to be converted: ")
check = NumbersConverter(numbers)
check.numbers_to_words()
