# gridcreation
my code for a grid of checkbuttons and ways to manipulate said checkbuttons
  
## Usage  
Firstly, import the class.  
Then, asign a variable to call the class with an x and y.  
There are some options which I will get into later
I usually call it grid1:  
```python  
import gridcreation as gc  
grid1 = gc.grid(20, 20)  
grid1.root.mainloop()
```  
From here on I will be asuming you called the variable grid1  
Now you have a grid of checkbuttons, we will now get into manipulating them.
grid1.boxlist is a list of all the checkbuttons, you can manipulate them like any other tkinter checkbutton.  
But how do you find the right checkbutton in this list?  
You can use grid1.coords([x,y]) this will return the corresponding index for the checkbutton in the boxlist and varlist.  
### The grid's x and y start at 1 and not actually at 0  
You also have grid1.varlist which is a list of IntVar()'s corresponding to the buttons.  
Once again they can be manipulated as expected and grid1.coords() can help
If you want to transform an index into the actually coordinates you can do grid1.uncoords(index).  
  
## grid() options  
xoffset: enables you to make all rows +something so you can place buttons before the grid.  
yoffset: see xoffset.  
text: text the buttons will start with.  
command: specify a command for the checkbuttons to start with.  
root: used to specify your own window mainly if you want to use Toplevel() instead of Tk().  
  
  
Thats about it, contact me if you have questions.  
Be sure to check out my projects with this!
