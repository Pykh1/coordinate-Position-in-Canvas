# coordinate-Position-in-Canvas
how we can Acces and capture the coordinate Position of mouse cursor over a widget is clicked usinf (event,handle)

from tkinter import*
my_window=Tk()
def display_coordinate(event):
    my_label["text"]=str(event.x)
my_canvas=Canvas(my_window,height=400,width=400,background="white")
my_label=Label(my_window,bd=2,font="times 18 bold",relief="solid",bg="white",fg="black")
my_canvas.bind('<Button-1>',display_coordinate)
my_canvas.grid(row=0,column=0)
my_label.grid(row=1,column=0)
my_window.mainloop()
