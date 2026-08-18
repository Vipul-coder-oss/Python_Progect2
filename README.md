# Python Digital Clock
I created a digital clock using Python
<br>
Author - Vipul Choudhary

"This project is built using Python and can be developed with the Tkinter library to create a simple and attractive graphical user interface (GUI)."

import tkinter as tk    
"tk is used for graphical user interface (GUI)"
from time import strftime 
"from is used for forward time or date acording to"

root=tk.Tk()
"root is used for crete object"

root.title("Digital clock")

def time():
    string=strftime('%H:%M:%S %p \n %D')
    label.config(text=string)
    label.after(1000,time)

label=tk.Label(root,font=('calibri',50,'bold'), background='black',foreground='white')

label.pack(anchor='center')


time()


root.mainloop()
