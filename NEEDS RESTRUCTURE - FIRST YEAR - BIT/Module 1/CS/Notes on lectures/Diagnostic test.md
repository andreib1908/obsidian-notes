
```Python
# Diagnostic Test  
  
def capitalize_each_word(text):  
    if not isinstance(text, str) or len(text) == 0:  
        print("Invalid Argument")  
        return None  
    else:  
        return text.title()  
  
  
def get_types(list_of_items):  
    if len(list_of_items) == 0:  
        print("Invalid Argument.")  
        return None  
    else:  
        for item in list_of_items:  
            print(type(item))  
  
  
def generate_password(length, qty_letters, qty_digits):  
    if isinstance(length, int) and isinstance(qty_letters, int) and isinstance(qty_digits,  
                                                                               int) and length > 0 and qty_letters > 0 and qty_digits > 0 and length > qty_letters + qty_digits:  
        qty_symbols = length - (qty_letters + qty_digits)  
        letters = string.ascii_letters  
        digits = string.digits  
        symbols = string.printable.replace(letters, "").replace(digits, "")  
        password = []  
  
        # letters  
        qty_counter = 0  
        while qty_counter < qty_letters:  
            random_letter = random.choice(letters)  
            password.append(random_letter)  
            qty_counter += 1  
  
        # digits  
        qty_counter = 0  
        while qty_counter < qty_digits:  
            random_digit = random.choice(digits)  
            password.append(random_digit)  
            qty_counter += 1  
  
        # symbols  
        qty_counter = 0  
        while qty_counter < qty_symbols:  
            random_symbol = random.choice(symbols)  
            password.append(random_symbol)  
            qty_counter += 1  
  
        loop = True  
        while loop:  
            previous_item = password[0]  
            for item in password:  
                if isinstance(item, type(previous_item)):  
                    random.shuffle(password)  
                    previous_item = item  
                else:  
                    break  
            loop = False  
  
        password = ''.join(password)  
  
        return password  
    else:  
        print("Invalid argument. Check specifications.")  
  
  
def merge_dictionaries(dict1, dict2):  
    if not dict1 or not dict2:  
        print("Invalid Argument.")  
        return None  
    else:  
        my_dict = {}  
        for key in dict1:  
            value = dict1.get(key)  
            if key in dict2:  
                value2 = dict2.get(key)  
                my_dict[key] = value + value2  
            else:  
                my_dict[key] = value  
  
        for key in dict2:  
            value = dict2.get(key)  
            if key not in dict1:  
                my_dict[key] = value  
        return my_dict  
  
  
roma_fans_dataset_1 = {  
    'Lazio': 430000,  
    'Abruzzo': 104000,  
    'Campania': 100000,  
    'Toscana': 150000  
}  
  
roma_fans_dataset_2 = {  
    'Lazio': 500000,  
    'Abruzzo': 154000,  
    'Campania': 230000  
}  
  
roma_fans_dataset = merge_dictionaries(roma_fans_dataset_1, roma_fans_dataset_2)
```