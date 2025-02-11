# OOPAsciiArt

**OOPAsciiArt** is an object-oriented Java application that converts images into ASCII art. The project leverages robust OOP and OOD principles to modularize the process of image handling, ASCII character matching, and user interaction.

---

## Project Overview

The application converts an input image into an ASCII art representation by:
- Loading and processing the image into a 2D pixel array.
- Padding and partitioning the image into sub-images according to a specified resolution.
- Computing the brightness of each sub-image and mapping it to an ASCII character from a configurable character set.
- Allowing users to interactively adjust parameters (e.g., character set, resolution, rounding method, and output format) via a command-line interface.

---

## Build and Run Instructions

1. **Compile the Project:**

   Ensure that your Java compiler is set up, then compile the source files:
   ```bash
   javac -d bin src/art_ascii/*.java src/image/*.java src/matching_char_image/*.java
Run the Application:

2. **Execute the main class (Shell) by providing the path to an image file as an argument:**

bash
Copy
java -cp bin art_ascii.Shell path/to/your/image.jpg
Interactive Commands:

3. **Once running, you can use the following commands in the interactive shell:**

exit – Exit the application.
chars – Display the current character set.
add <character|all|space|range> – Add characters to the set.
remove <character|range> – Remove characters from the set.
res [up|down] – Adjust the resolution.
output <html|console> – Switch the output format.
round <up|down|abs> – Change the rounding method for brightness matching.
asciiArt – Run the ASCII art conversion algorithm.
