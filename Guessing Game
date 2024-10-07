#include <iostream>
#include <cstdlib>
#include <ctime>

using namespace std;

void guessingGame() {
    int target, guess, lives = 10;
    srand(time(0));  // Seed for random number generator
    target = rand() % 100 + 1;  // Random number between 1 and 100

    cout << "Welcome to the guessing game" << endl;
    cout << "You have 10 lives. Each wrong guess will cost 1 life." << endl;

    while (lives > 0) {
        cout << "Guess a number: ";
        cin >> guess;

        if (guess < target) {
            cout << "The number is too low! Please try again." << endl;
            lives--;
        } else if (guess > target) {
            cout << "The number is too high! Please try again." << endl;
            lives--;
        } else {
            cout << "Congratulations! You guessed the number." << endl;
            break;
        }

        if (lives > 0) {
            cout << "You have " << lives << " lives left." << endl;
        } else {
            cout << "You've run out of lives! The correct number was " << target << "." << endl;
        }
    }
}

int main() {
    int choice;

    do {
        cout << "Please choose [1] [2]:" << endl;
        cout << "1. Enter a game" << endl;
        cout << "2. Exit" << endl;
        cout << "Choice: ";
        cin >> choice;

        if (choice == 1) {
            guessingGame();
        } else if (choice == 2) {
            cout << "Exiting the game. Goodbye!" << endl;
        } else {
            cout << "Invalid choice. Please choose again." << endl;
        }
    } while (choice != 2);

    return 0;
}