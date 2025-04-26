# Metadata-Extraction-using-ExifTool-log2timeline-and-Hidden-Data-Search-using-Steganography-Tools
### NAME : SUSINDHAR K M
### REGISTER NUMBER : 212223040218
## AIM:
To extract metadata, perform timeline analysis, and search for hidden data using forensic tools like ExifTool, log2timeline, and steganography detection tools.

## DESIGN STEPS:
### Step 1:
Use exiftool to extract metadata from files such as images, documents, and videos.

### Step 2:
Use log2timeline and plaso to create and analyze event timelines from system logs and file metadata.

### Step 3:
Apply steganography detection tools like steghide, zsteg, or binwalk to uncover hidden data in media files.

## PROGRAM:
Metadata and Timeline Forensics, Steganography Analysis Steps
# A. Using ExifTool – for file metadata

 Install:
```
sudo apt update
sudo apt install exiftool -y
```
 Extract metadata from a file:
```
exiftool image.jpg
```
 Batch process a folder:
```
exiftool -r /path/to/folder
```
Useful flags:

-G: Show metadata group

-time:all: Show only timestamps

-GPSLatitude -GPSLongitude: Extract GPS data

![image](https://github.com/user-attachments/assets/c36640f7-e35a-4946-8f51-2e616338573d)


# install log2timeline
```
sudo apt install plaso -y
```
```
sudo apt install steghide -y
```
# Embed data
```
steghide embed -cf /home/kali/Downloads/wallpaper.jpg -ef /home/kali/Downloads/secret.txt
```
![image](https://github.com/user-attachments/assets/bae809a0-5ab5-4241-aa62-aa172c3650be)



Extract hidden data:
```
steghide extract -sf hidden.jpg
```
![image](https://github.com/user-attachments/assets/7479df69-301e-485f-bcd7-96f398f7705a)


# Using binwalk – for file analysis

```
sudo apt install binwalk -y
binwalk suspicious.jpg
```
![image](https://github.com/user-attachments/assets/7bf1acdc-ca77-4526-81e9-8240df96cc6e)


## OUTPUT:
Extracted Metadata, Timeline Events, and Hidden Data Detection Results
![image](https://github.com/user-attachments/assets/4495d252-968f-4e02-927c-05a0a3760b00)


## RESULT:
Metadata was successfully extracted, timeline analysis was completed, and hidden data was identified using steganography tools.

