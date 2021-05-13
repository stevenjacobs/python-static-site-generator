# notes

## Module 1. The Site Class

directory = self.dest / path.relative_to(self.source)

    * The Path class has a __truediv__ method that returns another Path.
    * You can do the same with your own classes.

## Module 2. The Parser Class

extensions: List[str] = []

    * This is called an `annotation` of an empty List.

## Module 3. The Content Class

Lots of interesting things going on here:

classmethod

    * load() is a classmethod. Classmethods are used as factories that return a class object for different use cases. 
        It is similar to other languages where functions with the same name are overloaded, and where the compiler knows which function to used based on the arguments alone. E.g. when a string, integer or object is passed.

        A classmethod is also used with inheritance to ensure that the object that is created is an object of a child class.
        A staticmethod does similar things than a classmethod. 
        However, a staticmethod from a parent class always returns an object of that base class. 
        A classmethod creates an instance of the child class if it was called on that child class.

        See: https://www.programiz.com/python-programming/methods/built-in/classmethod