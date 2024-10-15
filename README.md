Rsyncer 

Folder Duplication Script

This Zsh script duplicates a folder using `rsync`, removes unwanted `.DS_Store` files, and displays a summary of the copied files and their size.

 Features

- Drag-and-drop folder selection via the macOS application interface.
- Validates the folder path and checks if the folder exists.
- Automatically removes `.DS_Store` files from the source and destination folders.
- Uses `rsync` to copy the folder while preserving metadata.
- Displays a summary of the total files copied and their size (GB or MB).
- Shows error messages if the folder is invalid or already exists on the desktop.

 Script Overview

The script follows these steps:

1. Get the Folder Path: The application accepts the folder path via drag-and-drop in the app interface.
2. Validate Input: If no folder is provided, the script exits silently. If the folder path is invalid or does not exist, it displays an error message.
3. Clean Up `.DS_Store` Files: Removes `.DS_Store` files from both the source and destination folders.
4. Folder Duplication: Uses `rsync` to copy the folder to the desktop, appending "rsync folder" to the destination folder name.
5. Error Handling: Displays error messages for issues like invalid folder paths or if the destination folder already exists.
6. Summary Display: After a successful copy, calculates the total size of the files and displays the number of files copied along with their total size in GB or MB.

 Installation and Usage

1. Download the macOS application created using Platypus (you do not need Platypus installed to run the app).
2. Run the application by double-clicking it.
3. Drag and drop a folder into the application window to start the duplication process.
4. The folder will be copied to your desktop with a new name that appends "rsync folder".
5. After the process completes, a summary dialog will display the total files copied and the total size.

 Command-line Usage (Optional)

If you prefer to run the underlying script directly from the command line (without using the macOS app), you can:

```bash
./your-script-name.zsh "/path/to/source/folder"
Where /path/to/source/folder is the absolute path of the folder you want to duplicate.

Example

If the script is used on a folder located at /Users/yourusername/Documents/ImportantFolder, and the folder contains 100 files with a total size of 500 MB, the script will:

Copy the folder to your Desktop, renaming it to "ImportantFolder rsync folder".
Remove all .DS_Store files from both the source and destination folders.
Display a dialog with a message like:
mathematica
Copy code
Folder duplicated successfully! 
Total files copied: 100 
Total size: 500 MB
Error Handling

If the source folder does not exist, a dialog will display an error message.
If the destination folder already exists, the script will show an error and prevent overwriting.
If the rsync operation fails, an error message will be displayed.
Contributing

Feel free to submit issues or pull requests for improvements or bug fixes. Contributions are welcome!


Note: Users do not need Platypus installed to use the application; it functions as a standalone app.
