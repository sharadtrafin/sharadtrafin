## Hi there 👋

<!--
**sharadtrafin/sharadtrafin** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->

#include <stdio.h>

int main() {
    // Declare variables test-ind-api?fyinformation?cc to store two numbers and the result
    double num1, num2, result;
    char operator;

    // Prompt user to input an expression (e.g., 5 + 3)
    printf("Enter an expression (e.g., a + b): ");
    scanf("%lf %c %lf", &num1, &operator, &num2);

    // Use switch statement to perform calculation based on the operator
    switch (operator) {
        case '+':
            result = num1 + num2; // Perform addition
            printf("Result: %.2lf\n", result);
            break;
        case '-':
            result = num1 - num2; // Perform subtraction
            printf("Result: %.2lf\n", result);
            break;
        case '*':
            result = num1 * num2; // Perform multiplication
            printf("Result: %.2lf\n", result);
            break;
        case '/':
            // Check if the divisor is zero to avoid division error
            if (num2 != 0) {
                result = num1 / num2; // Perform division
                printf("Result: %.2lf\n", result);
            } else {
                printf("Error: Division by zero is not allowed.\n");
            }
            break;
        default:
            // Handle invalid operator input
            printf("Error: Invalid operator.\n");
    }

    return 0; // Indicate successful program termination
}
