# RobotDodge Game with Inheritance

This project demonstrates the use of inheritance in C# to create a dynamic gaming environment with multiple types of robots. It leverages the power of hierarchical code organization to enhance game development.

## Project Overview

### Objective

The objective of this project is to:
1. Implement inheritance to create different kinds of robots in the RobotDodge game.
2. Use abstract classes and method overriding to change the way each robot type is drawn.

### Files Included

- `Robot.cs`
- `RobotDodge.cs`

### Instructions Followed

1. **Robot Class Enhancements**:
    - **File**: `Robot.cs`
    - **Steps**:
        1. Create a new class `Boxy` inheriting from the `Robot` class.
        2. Move the `Draw` method code from the `Robot` class into the `Boxy` class and add a new abstract `Draw` method to the `Robot` class.
        3. Change the `Robot` class to be abstract.
        4. Add a constructor to the `Boxy` class that accepts a `Window` and passes it to the `Robot` constructor.
        5. Update the `RandomRobot` method in `RobotDodge` to return a new `Boxy` object.
        
2. **Adding Roundy Class**:
    - **File**: `Robot.cs`
    - **Steps**:
        1. Create a `Roundy` class with an appropriate constructor.
        2. Implement the `Draw` method for `Roundy` with the provided code.
        3. Update the `RandomRobot` method to create a `Boxy` 50% of the time and a `Roundy` 50% of the time.

### Key Features

- **Inheritance and Abstraction**: Utilize inheritance to create an abstract `Robot` class and concrete `Boxy` and `Roundy` classes.
- **Method Overriding**: Implement different drawing methods for each robot type using method overriding.
- **Dynamic Robot Creation**: Easily extend the game by adding new types of robots with minimal code changes.

### Demonstration

- **Adding Boxy Robot**:
    1. Created a `Boxy` class inheriting from `Robot`.
    2. Implemented the `Draw` method for `Boxy`.
    3. Added a constructor to `Boxy` to pass the `Window` to the base `Robot` constructor.
    4. Updated the `RandomRobot` method to return `Boxy`.

- **Adding Roundy Robot**:
    1. Created a `Roundy` class inheriting from `Robot`.
    2. Implemented the `Draw` method for `Roundy` using the provided drawing logic.
    3. Updated the `RandomRobot` method to create `Boxy` 50% of the time and `Roundy` 50% of the time.

- **Adding Custom Robot**:
    1. Created a new custom robot class.
    2. Implemented the `Draw` method for the custom robot.
    3. Updated the `RandomRobot` method to include the custom robot.

## How to Run the Program

1. **Compile the Program**:
    ```bash
    csc Robot.cs RobotDodge.cs
    ```
2. **Run the Program**:
    ```bash
    RobotDodge.exe
    ```

### Technologies Used

- `C#`
- `SplashKit` (for drawing and game development)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


