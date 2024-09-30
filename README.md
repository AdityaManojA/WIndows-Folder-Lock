
# Coding Quiz Competition - Folder Lock Challenge

## Overview

Welcome to the **Coding Quiz Competition**! This competition involves a unique folder-locking mechanism using a batch script (`.bat` file) to secure important files during different stages of the quiz. Participants will lock and unlock folders by providing the correct password to proceed to the next stage.

### How It Works
The batch file provided will lock a folder named `Private` and hide it from view. To access the contents, participants will need to unlock the folder by entering the correct password. Successfully unlocking the folder allows participants to retrieve a key or file that will help them proceed to the next stage of the quiz.

## Instructions

### Setup

1. **Download the Script**: Download or copy the batch file (`quiz-locker.bat`) onto your Windows system.

2. **Edit the Password**: Open the batch file in a text editor and replace `YOUR-PASSWORD` with a password of your choice that participants need to unlock the folder. Example:

   ```batch
   if NOT %pass%== YOUR-PASSWORD goto FAIL
   ```

   Replace `YOUR-PASSWORD` with the desired password.

3. **Create the Folder**: Run the batch file. This will create a folder called `Private` in the same directory if it does not already exist.

4. **Add the Quiz Files**: Place the key, next clue, or quiz-related files inside the `Private` folder.

### How to Use the Batch File

- **Locking the Folder**:  
  To lock the folder, run the batch file and choose `Y` when prompted:
  
  ```
  Are you sure to lock this folder? (Y/N)
  ```

  The folder will be renamed and hidden, making it inaccessible.

- **Unlocking the Folder**:  
  To unlock the folder, run the batch file again. You will be prompted to enter the password:
  
  ```
  Enter password to Unlock Your Secure Folder
  ```

  If the correct password is entered, the folder will be unlocked, and you will be able to access the contents.

- **Failed Attempts**:  
  If an incorrect password is entered, the batch file will display:
  
  ```
  Invalid password
  ```

### Batch File Explanation

- The script locks and hides the `Private` folder by renaming it with a system class identifier for the Windows Control Panel and applying the hidden and system attributes.
- Unlocking the folder requires a password that the user must input. If the correct password is provided, the folder is made visible again.
  
### Notes

- This method is not foolproof and should not be used for sensitive data as it only applies basic protection by hiding the folder.
- The folder lock mechanism works on **Windows** systems only.
- Ensure you set the correct password before sharing the batch file for the competition.

### Troubleshooting

- If the folder does not appear after unlocking, try refreshing the directory or disabling any hidden folder settings in your Windows Explorer.
- If the batch script doesn't work as expected, ensure that you are running it with sufficient permissions (Administrator rights may be required for some systems).

### Disclaimer

This script is intended for educational purposes and light protection for a coding quiz competition. It should not be relied upon for securing sensitive or critical data.

Good luck with your quiz competition, and may the best coder win!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## MIT License

```plaintext
MIT License

Copyright (c) [2024] [Aditya Manoj]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


