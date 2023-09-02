#!/usr/bin/python3

def factorize(number):
    factors = []
    divisor = 2
    while divisor <= number:
        if number % divisor == 0:
            factors.append(divisor)
            number //= divisor
        else:
            divisor += 1
    return factors

def main():
    input_file = "prime_numbers"

    try:
        with open(input_file, 'r') as file:
            for line in file:
                number = int(line.strip())
                factors = factorize(number)
                factors_str = '{0}='.format(number) + '*'.join(map(str, factors))
                print(factors_str)
    except FileNotFoundError:
        print("Error: File '{0}' not found.".format(input_file))

if __name__ == "__main__":
    main()
