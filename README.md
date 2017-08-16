# Calculator a simple python calculator for a windows 64 bit system

from tkinter import *
from math import *
root=Tk()

#the functions
def add_0():
    string.set(string.get()+"0")
def add_1():
    string.set(string.get()+"1")
def add_2():
    string.set(string.get()+"2")
def add_3():
    string.set(string.get()+"3")
def add_4():
    string.set(string.get()+"4")
def add_5():
    string.set(string.get()+"5")
def add_6():
    string.set(string.get()+"6")
def add_7():
    string.set(string.get()+"7")
def add_8():
    string.set(string.get()+"8")
def add_9():
    string.set(string.get()+"9")
def addition():
    string.set(string.get()+"+")
def subtract():
    string.set(string.get()+"-")
def equals():
    x=eval(string.get())
    string.set(x)
def multiply():
    string.set(string.get()+"*")
def divide():
    string.set(string.get()+"/")
def exponentation():
    string.set(string.get()+"**")
def Square_root():
    string.set("sqrt("+string.get()+")")
def Cubic_root():
    string.set("pow("+string.get()+",1/3)")
def bracket_1():
    string.set(string.get()+"(")
def bracket_2():
    string.set(string.get()+")")
def Dot():
    string.set(string.get()+".")
def Restart():
    string.set(" ")
string=StringVar()
string.set(" ")
label=Label(root,textvariable=string)
label.grid(row=0,columnspan=7,sticky="n,e,w,s")

#The buttons

button_Add_0=Button(root,text="0",command=add_0)
button_Add_0.grid(row=1,column=0,sticky="n,e,w,s")

button_Add_1=Button(root,text="1",command=add_1)
button_Add_1.grid(row=1,column=1,sticky="n,e,w,s")

button_Add_2=Button(root,text="2",command=add_2)
button_Add_2.grid(row=1,column=2,sticky="n,e,w,s")

button_Add_3=Button(root,text="3",command=add_3)
button_Add_3.grid(row=1,column=3,sticky="n,e,w,s")

button_Add_4=Button(root,text="4",command=add_4)
button_Add_4.grid(row=1,column=4,sticky="n,e,w,s")

button_Add_5=Button(root,text="5",command=add_5)
button_Add_5.grid(row=1,column=5,sticky="n,e,w,s")

button_Add_6=Button(root,text="6",command=add_6)
button_Add_6.grid(row=1,column=6,sticky="n,e,w,s")

button_Add_7=Button(root,text="7",command=add_7)
button_Add_7.grid(row=1,column=7,sticky="n,e,w,s")

button_Add_8=Button(root,text="8",command=add_8)
button_Add_8.grid(row=1,column=8,sticky="n,e,w,s")

button_Add_9=Button(root,text="9",command=add_9)
button_Add_9.grid(row=1,column=9,sticky="n,e,w,s")

button_Addition=Button(root,text="+",command=addition)
button_Addition.grid(row=2,column=0,sticky="n,e,w,s")

button_Subtraction=Button(root,text='-',command=subtract)
button_Subtraction.grid(row=2,column=1,sticky="n,e,w,s")

button_Multiply=Button(root,text="*",command=multiply)
button_Multiply.grid(row=2,column=2,sticky="n,e,w,s")

button_Division=Button(root,text="/",command=divide)
button_Division.grid(row=2,column=3,sticky="n,e,w,s")

button_Exponentation=Button(root,text="^",command=exponentation)
button_Exponentation.grid(row=2,column=4,sticky="n,e,w,s")

button_Square_Root=Button(root,text="sqrt",command=Square_root)
button_Square_Root.grid(row=2,column=5,sticky="n,e,w,s")

button_Cubic_root=Button(root,text="cubrt",command=Cubic_root)
button_Cubic_root.grid(row=2,column=6,sticky="n,e,w,s")

button_Bracket_1=Button(root,text="(",command=bracket_1)
button_Bracket_1.grid(row=2,column=7,sticky="n,e,w,s")

button_Bracket_2=Button(root,text=")",command=bracket_2)
button_Bracket_2.grid(row=2,column=8,sticky="n,e,w,s")

button_Dot=Button(root,text=".",command=Dot)
button_Dot.grid(row=2,column=9,sticky="n,e,w,s")

button_Equals=Button(root,text="=",command=equals)
button_Equals.grid(row=0,column=8,sticky="n,e,w,s")

button_Restart=Button(root,text="Restart",command=Restart)
button_Restart.grid(row=0,column=9,sticky="n,e,w,s")

root.mainloop()
