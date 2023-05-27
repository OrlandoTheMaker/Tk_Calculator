# Tk_Calculator
Tkinter Calculator  In Python


# Importing the necessary libraries
import tkinter as tk



# Defining the Calculator class
class Calculator:
    def __init__(self, master):
        self.master = master
        master.title("Python Calculator")
 
 
 
# Creating the display widget
self.display = tk.Entry(master, width=40, borderwidth=5)
self.display.grid(row=0, column=0, columnspan=4, padx=10, pady=10)




# This code creates an Entry widget (a text input field) that will be used to display the calculator input and output. It is placed in the first row and spans across all four columns.

# Creating the number buttons
self.button_1 = tk.Button(master, text="1", padx=40, pady=20, command=lambda: self.button_click(1))
...
self.button_0 = tk.Button(master, text="0", padx=40, pady=20, command=lambda: self.button_click(0))



# These lines create the buttons for numbers 0-9. Each button is created using the Button widget and is assigned a number as its text. The padx and pady arguments specify the padding around the button. The command argument assigns a function to be called when the button is clicked. In this case, we use a lambda function to call the button_click() method with the corresponding number as an argument.

# Creating the operator buttons:
self.button_add = tk.Button(master, text="+", padx=39, pady=20, command=self.button_add)
...
self.button_divide = tk.Button(master, text="/", padx=41, pady=20, command=self.button_divide)



# These lines create the buttons for addition, subtraction, multiplication, and division. Similar to the number buttons, each button is assigned a text and a command function.

# Creating the clear and equals buttons:
self.button_clear = tk.Button(master, text="Clear", padx=79, pady=20, command=self.button_clear)
self.button_equals = tk.Button(master, text="=", padx=91, pady=20, command=self.button_equals)



# These lines create the buttons for clearing the display and calculating the result. The text and command functions are specified in a similar manner.

# Positioning the buttons on the screen:
self.button_1.grid(row=1, column=0)
...
self.button_equals.grid(row=5, column=0, columnspan=4)



# These lines use the grid() method to position the buttons in a grid layout. The row and column arguments determine the position of each button. Additionally, the columnspan argument is used to make the equals button span across all four columns.


# So this is basically the structure of a GUI calculator with tkinter python. 
# It creates a window with a display and a grid of buttons. 
# Each button is associated with a specific function to handle user interactions. 
# You can further extend this code to add more functionality or enhance the design of the calculator.
