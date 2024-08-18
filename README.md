# GUIDartScorer
import tkinter as tk


def score():
  list = []
  list.append(int(entry.get()))
  root = tk.Tk()
  listbox = tk.Listbox(root)
  for item in list:
    listbox.insert(tk.END, item)
  listbox.pack()


# Create the main window
window = tk.Tk()
window.title("score tracker")

# Create a label
label = tk.Label(window, text="Enter your score")
label.pack()

# Create an entry field
entry = tk.Entry(window)
entry.pack()


# Create a button
button = tk.Button(window, text="add", command=score)
button.pack()

# create a second label
label1 = tk.Label(window, text="wanna see your score?")
label1.pack()



# Start the GUI event loop
window.mainloop()
