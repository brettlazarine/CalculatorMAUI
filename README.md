## **CalculatorMAUI**

A project focused on Style led by Hector Perez on his Udemy course: *.NET MAUI course with Visual Studio 2022 creating PROJECTS*

The XAML is designed in the layout of a typical cell phone calculator, keypad at the bottom and results at the top. The buttons each use Commands to achieve their part of calculating whatever equation the user wants.
The Style for the application is achieved by way of *CalcDictionary*, a Style dictionary that defines the aesthetic of the various Controls. Phone dark and light themes are also taken into consideration, with AppThemeBinding implemented into the Style Dictionary to ensure the application will function regardless of the user's theme settings.

The ViewModel achieves the calculator functionality for the app:
- *OperationCommand* adds the desired number/operand to *Formula* for calculation
- *ResetCommand* returns *Result* and *Formula* to their default values
- *BackspaceCommand* removes the last indexed value from *Formula*
- *CalculateCommand* implements the *Dangl.Calculator* NuGet Package and calculates the result of the user's input
