# jelajahbug

def calculate_sum(numbers):
    total = 0
    for num in numbers:
        total += num
    return total

def test_calculate_sum():
    test_cases = [
        ([1, 2, 3], 6),
        ([4, 5, 6], 15),
        ([], 0),
        ([10, -5, 3], 8)
    ]
    for numbers, expected_result in test_cases:
        result = calculate_sum(numbers)
        if result != expected_result:
            print(f"Bug found! Expected {expected_result}, but got {result} for input {numbers}")

test_calculate_sum()
