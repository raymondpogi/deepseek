Prompt for AI:

Objective: Create a PowerShell script with a graphical user interface (GUI) that allows users to search for files and folders, display the results in a list, and organize the results by size. The script should also include a button to open the selected file's location in File Explorer.

Requirements:

Form-Based GUI:

Use System.Windows.Forms to create a form with a textbox, buttons, and a list view.

The form should have a title, such as "File and Folder Search".

Search Functionality:

Allow the user to input a drive or folder path manually or via a "Browse" button.

When the "Search" button is clicked, the script should recursively search the specified path for files and folders.

Display the results in a ListView with columns for "Name", "Full Path", and "Size (MB)".

Organize by Size:

Add a button labeled "Organize by Size" that sorts the results in the ListView by file size in ascending order.

Ensure the sorting is numeric (not alphabetical) for the "Size (MB)" column.

Go to File Location:

Add a button labeled "Go to File Location" that opens the folder containing the selected file in File Explorer and highlights the file.

The button should only be enabled when a file is selected in the ListView.

Error Handling:

Handle errors gracefully, such as invalid paths or inaccessible folders.

Display appropriate error messages to the user.

Administrator Privileges:

Ensure the script runs with Administrator privileges to access all folders.

Additional Notes:

Use Add-Type -AssemblyName System.Windows.Forms and Add-Type -AssemblyName System.Drawing to load the necessary assemblies.

Avoid using Add-Type for custom comparers; instead, implement sorting directly in PowerShell.

The script should be self-contained and easy to run.

Example Output:

A PowerShell script that creates a GUI with the specified functionality.

The script should be well-commented and easy to understand.
