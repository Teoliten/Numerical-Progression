# Numerical Progression
This C++ program implements a hierarchy of numerical progressions using object-oriented programming concepts. It includes an abstract base class `Progression` and three derived classes representing arithmetic, geometric, and harmonic progressions.

## Class Abstraction
Class abstraction is a fundamental concept in object-oriented programming that allows you to define abstract classes with pure virtual functions. In this project, the `Progression` class is an abstract class that defines the common interface for all numerical progressions, providing a blueprint for its derived classes.

## Inheritance
Inheritance is a key feature of object-oriented programming that allows a class to inherit properties and behaviors from another class. Here, the derived classes (`ArithmeticPr`, `GeometricPr`, `HarmonicPr`) inherit from the Progression base class, reusing and extending its functionality while maintaining a clear and organized class hierarchy.

## Polymorphism
Polymorphism is demonstrated through the use of virtual functions. The `Progression` class declares a pure virtual function `nextValue()`, and each derived class provides its own implementation. In the `main` function, polymorphism is showcased when calling `nextValue()` on instances of different derived classes through a common base class pointer.

Feel free to explore and modify the code to enhance your understanding of these object-oriented programming concepts.

## Classes
### Progression (Base Class)
The `Progression` class serves as the base class for numerical progressions. It includes a constructor to initialize the starting point and a pure virtual function for generating the next value in the progression.

Member Functions
- `Progression(long start = 0)`: Constructor that initializes the current value of the progression.
- `long firstValue()`: Returns the first value in the progression.
- `virtual long nextValue() = 0`: Pure virtual function to generate the next value in the progression.

### ArithmeticPr (Derived Class)
The `ArithmeticPr` class represents an arithmetic progression, where each value is obtained by adding a common difference to the previous value.

Member Functions
- `ArithmeticPr(long start = 0, long value = 1)`: Constructor that initializes the starting point and the common difference.
- `long nextValue()`: Generates the next value in the arithmetic progression by adding the common difference.

### GeometricPr (Derived Class)
The `GeometricPr` class represents a geometric progression, where each value is obtained by multiplying the previous value by a common ratio.

Member Functions
- `GeometricPr(long start = 0, long value = 1)`: Constructor that initializes the starting point and the common ratio.
- `long nextValue()`: Generates the next value in the geometric progression by multiplying the common ratio.

### HarmonicPr (Derived Class)
The `HarmonicPr` class represents a harmonic progression, where each value is obtained by incrementing the previous value.

Member Functions
- `HarmonicPr(long start = 1)`: Constructor that initializes the starting point.
- `long nextValue()`: Generates the next value in the harmonic progression by incrementing the current value.

## Usage
The `main` function demonstrates the usage of these progression classes by creating instances of each and printing the first five values for each progression type.

```cpp
ArithmeticPr ap(5, 1);   // Arithmetic progression: Start at 5, addition with 1 each time.
GeometricPr gp(10, 2);   // Geometric progression: Start at 10, multiply with 2 each time.
HarmonicPr hp(1);        // Harmonic progression: Start at 1, 1/2, 1/3, 1/4, 1/5 etc.

// Generate and print the first 5 values in each progression
// ...
```
Feel free to extend and modify the code according to your specific requirements.
