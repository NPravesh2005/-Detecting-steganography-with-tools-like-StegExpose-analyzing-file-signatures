# EX 8 : Detecting-steganography-with-tools-like-StegExpose-analyzing-file-signatures
## AIM:
To detect hidden data using steganography detection tools like StegExpose and analyze file signatures for authenticity and manipulation.

## DESIGN STEPS:
### Step 1:
Install StegExpose or use the JAR version to detect steganography in image files.

### Step 2:
Run StegExpose on a directory of suspected image files using the command:

### Step 3:
Analyze file signatures using tools like file, binwalk, or xxd to check for inconsistencies or embedded content.

## PROCEDURE:
StegExpose and File Signature Analysis Commands

# Step 1: Download Image and Create Secret Message File
• Download a .jpeg image  from a trusted website or use own image.

<img width="1919" height="1079" alt="Screenshot 2025-10-04 090512" src="https://github.com/user-attachments/assets/9f575e3c-8269-45b3-8322-e9c517384f6b" />


• Create a text file named secret with a confidential message:

<img width="1918" height="996" alt="Screenshot 2025-10-04 090704" src="https://github.com/user-attachments/assets/74d2a3f5-fbf2-4ff4-8442-e2ad1a6b6bb0" />


# Step 2: Install and Verify Steghide Tool
• To install Steghide on Parrot OS,run:

• Confirm the installation by checking its version:

<img width="427" height="135" alt="Screenshot 2025-10-04 090747" src="https://github.com/user-attachments/assets/54a6fee9-52c0-4234-b7be-5b10e67cf916" />


# Step 3: Embed the Secret Message into the Image
• Use the following command to embed secret into lion.jpg:

<img width="799" height="479" alt="Screenshot 2025-10-04 091236" src="https://github.com/user-attachments/assets/3c717cac-f38c-4348-b37d-43316c8ba1cb" />


# Step 4: Delete the Original Secret File
• After embedding, delete the plaintext file:

<img width="547" height="148" alt="Screenshot 2025-10-04 091323" src="https://github.com/user-attachments/assets/e9f7a874-a9ed-45e6-a004-b15bfdcaa211" />



## OUTPUT:
List of Images with Steganography Detection Scores and File Signature Details

# Step 1: Extract the Embedded Secret from the Image

<img width="951" height="744" alt="Screenshot 2025-10-04 091505" src="https://github.com/user-attachments/assets/2e88096e-e647-4b5b-837e-d9537caea96d" />


• To retrieve the hidden file: • Enter the same passphrase used during embedding.

<img width="813" height="715" alt="Screenshot 2025-10-04 091651" src="https://github.com/user-attachments/assets/4f62adc0-9a3b-4fff-88ab-1e5e0b7d8e22" />


# Step 2: Verify the Extracted Message
• Display the extracted file content to verify:

• Ensure the message matches the original secret content.

• Another command to see the same secret message is

# Step 3: Retrieve Information About the Embedded Data
• To gather details about embedded content in the image:

<img width="803" height="370" alt="Screenshot 2025-10-04 091751" src="https://github.com/user-attachments/assets/38be7a3e-2647-48af-b6cd-8c99ae32b4b1" />


• This will display file type, size, and whether data is embedded.
## RESULT:
Hidden data was successfully detected and file signatures were analyzed for irregularities.
