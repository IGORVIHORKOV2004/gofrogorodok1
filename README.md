# gofrogorodok1
import tkinter
master = tkinter.Tk()
canvas = tkinter.Canvas(master, bg='white', height=400, width=400)
k=400/8
v=4*4
for i in range(8):
        x = i * k
        canvas.create_line((x, 0), (x,400), fill='black')
        canvas.create_line((0, x), (400, x), fill='black')
for a in range(8):
        b=v
        canvas.create_circle((b,0),(b,400),fill="blue")
        canvas.create_circle((0,b),(400,b), fill="green")
canvas.pack()
master.mainloop()
