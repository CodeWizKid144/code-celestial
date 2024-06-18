# code-celestial
codemoon
import random

def generate_random_matrix(n):
    matrix = []
    for i in range(n):
        row = []
        for j in range(n):
            row.append(random.randint(1, 100))  # Генеруємо випадкове число від 1 до 100
        matrix.append(row)
    return matrix

def print_matrix(matrix):
    for row in matrix:
        print(row)

# Використання функцій для генерації та виведення матриці 5x5
n = 5  # Розмір матриці
random_matrix = generate_random_matrix(n)
print("Randomly Generated Matrix:")
print_matrix(random_matrix)
