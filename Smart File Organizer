import os       # OS module is used for interacting with the operating system (file paths, listing directories, etc.)
import shutil   # shutil module is used to move or copy files

# Step 1: Ask user to enter the folder path where files need to be organized
path = input("Enter Your Path -> ")

# Step 2: List all files and folders inside the given path
file = os.listdir(path)

# Step 3: Loop through each file in the folder
for i in file:
    # Step 4: Split the file name and its extension (e.g., 'photo.jpg' -> 'photo', '.jpg')
    filename, extension = os.path.splitext(i)

    # Step 5: Remove the dot from extension (e.g., '.jpg' becomes 'jpg') for folder naming
    extension_1 = extension[1:]

    # Optional: You can uncomment this to see the extension being processed
    # print(extension_1)

    # Step 6: Create path for the folder named after the extension
    folder_path = path + "\\" + extension_1

    # Step 7: Check if folder for that extension already exists
    if os.path.exists(folder_path):
        # Step 8: If folder exists, move the file into that folder
        shutil.move(path + "\\" + i, folder_path + "\\" + i)
    else:
        # Step 9: If folder doesn't exist, create the folder
        os.makedirs(folder_path)

        # Step 10: Move the file into the newly created folder
        shutil.move(path + "\\" + i, folder_path + "\\" + i)
