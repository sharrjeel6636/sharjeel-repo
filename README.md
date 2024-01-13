# sharjeel-repo
sharjeel  new repo
#include <stdio.h>
#include <math.h>

// Basic Operations
double add(double a, double b) {
    return a + b;
}

double subtract(double a, double b) {
    return a - b;
}

double multiply(double a, double b) {
    return a * b;
}

double divide(double a, double b) {
    if (b != 0) {
        return a / b;
    } else {
        printf("Error: Division by zero\n");
        return 0.0;
    }
}

// Trigonometric Operations
double sine(double angle) {
    return sin(angle);
}

double cosine(double angle) {
    return cos(angle);
}

double tangent(double angle) {
    return tan(angle);
}

// Algebraic Operations
double exponentiation(double base, double exponent) {
    return pow(base, exponent);
}

double squareRoot(double number) {
    if (number >= 0) {
        return sqrt(number);
    } else {
        printf("Error: Square root of a negative number\n");
        return 0.0;
    }
}

// Logarithmic Operations
double logarithm(double number) {
    if (number > 0) {
        return log10(number);
    } else {
        printf("Error: Logarithm of a non-positive number\n");
        return 0.0;
    }
}

double naturalLogarithm(double number) {
    if (number > 0) {
        return log(number);
    } else {
        printf("Error: Natural logarithm of a non-positive number\n");
        return 0.0;
    }
}

int main() {
    // Example usage
    double result;

    // Basic Operations
    result = add(5.0, 3.0);
    printf("Addition: %.2f\n", result);

    result = subtract(5.0, 3.0);
    printf("Subtraction: %.2f\n", result);

    result = multiply(5.0, 3.0);
    printf("Multiplication: %.2f\n", result);

    result = divide(5.0, 3.0);
    printf("Division: %.2f\n", result);

    // Trigonometric Operations
    double angle = 30.0; // Angle in degrees
    printf("Sine(%f): %.2f\n", angle, sine(angle));

    // Algebraic Operations
    result = exponentiation(2.0, 3.0);
    printf("Exponentiation: %.2f\n", result);

    result = squareRoot(9.0);
    printf("Square Root: %.2f\n", result);

    // Logarithmic Operations
    result = logarithm(100.0);
    printf("Logarithm (base 10): %.2f\n", result);

    result = naturalLogarithm(2.0);
    printf("Natural Logarithm (base e): %.2f\n", result);

    return 0;
}
