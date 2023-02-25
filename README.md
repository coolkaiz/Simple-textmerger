# Simple-testfile-merger
Here's how it works:
First, we define the merge_files function, which is called when the user clicks the "Merge Files" button.
This function uses filedialog.askdirectory to prompt the user to select a folder to merge files from.
       
    1. If the user cancels the dialog or doesn't select a folder, the function returns without doing anything. 
    2. If the user selects a folder, the function sets the output file name to be the same as the folder name with a .txt extension.
    3. The function then opens the output file in write mode ('w'), loops over all the files in the selected folder using os.listdir, and for each file, if it ends with the .txt extension, reads its contents and writes them to the output file with a newline character \n added to the end.
    4. Finally, the function shows a message box to let the user know that the merge is complete.
    5. We create the main window using tk.Tk, set its title to "Text File Merger", and create a button using tk.Button that calls the merge_files function when clicked. We pack the button using the pack method to add it to the window.
    6. Finally, we run the main loop using root.mainloop to start the GUI.

When you run the program, it will display a simple window with a "Merge Files" button.
Clicking this button will prompt the user to select a folder to merge files. 
