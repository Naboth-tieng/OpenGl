# OpenGL Translation Example

This simple C++ program demonstrates translation in OpenGL using GLUT. The program initializes a window and draws a diamond shape. It then translates the diamond by a specified distance and draws it again.

## Instructions

Follow the steps below to compile and run the program:

### Prerequisites

- Make sure you have a compatible C++ compiler installed on your system.
- Ensure that the OpenGL and GLUT libraries are available.

### Compilation

1. Clone or download the repository.

```bash
git clone <repository_url>
cd <repository_directory>
```

2. Compile the program using your preferred C++ compiler.

```bash
g++ -o translation_example translation_example.cpp -lopengl32 -lglu32 -lfreeglut
```

### Execution

Run the compiled executable.

```bash
./translation_example
```

## Code Overview

The source code (`translation_example.cpp`) consists of the following key components:

### Initialization

The `initGL` function initializes OpenGL settings, sets up the projection matrix, and defines the background color.

```cpp
void initGL() {
    // ... (code for initialization)
}
```

### Translation Function

The `drawTranslatedDiamond` function draws a diamond shape and translates it based on the specified parameters.

```cpp
void drawTranslatedDiamond(GLdouble a, GLdouble b) {
    // ... (code for drawing and translation)
}
```

### Display Function

The `display` function calls the translation function twice, showcasing the diamond before and after translation.

```cpp
void display() {
    // ... (code for calling drawTranslatedDiamond with different parameters)
}
```

### Main Function

The `main` function sets up the GLUT window and initializes the event loop.

```cpp
int main(int argc, char** argv) {
    // ... (code for GLUT initialization and event loop)
}
```

## Customize the Translation

Feel free to modify the `drawTranslatedDiamond` function parameters in the `display` function to experiment with different translation values.

```cpp
void display() {
    drawTranslatedDiamond(0.0, 0.0);     // Original position
    drawTranslatedDiamond(200.0, 200.0); // Translated position
}
```

Explore the possibilities of OpenGL translation by adjusting the translation distances in these function calls.

Have fun experimenting with OpenGL translation in this example!