import csv
from Tkinter import *

root = Tk()
#This function reads through the Capitals.csv file (States and their capital cities)

def query():
    with open('Challanges/Capitals.csv') as csvfile:
        place = csv.reader(csvfile, delimiter=',')
#If the STDin is the Capital City, STDout is the State.
        for row in place:
            if Field.get == row[1]:
                print('%s is in %s'%(Field(), row([0])).join(row))
#If the STDin is the state, STDout is the capital city.
            elif Field == row[0]:
                print('The capital city of %s is in %s'% (Field(), row([1])).join(row))
            else:
                print("Try again")


#***** GUI  *****
question = Label(root, text = "Enter one field and get the other. Remember to start with capslock ON")
Field = Entry(root)
Query=Label(root, text="Enter a state or Capital City:")


Query.grid(row=1,column=0, sticky=W)
question.grid(row=0,columnspan=4)
Field.grid(row=1, column=1, sticky=W)

Button(root, text='Quit', command=root.quit).grid(row=3, column=0, sticky=W, pady=1)
Button(root, text='Enter', command=query).grid(row=3, column=1, sticky=W, pady=1)
mainloop()
