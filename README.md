# Archive Project

## Project Overview
This project demonstrates how to create a structured directory, populate it with files, archive the directories, and compress the archive. It also covers how to extract and verify the contents of the archive.

## Step-by-Step Instructions

### 1. Set Up the Project Directory Structure

**Create a Main Project Directory:**

mkdir ArchiveProject
cd ArchiveProject

### 2. Set Up the Project Directory Structure

Create the following subdirectories within the ArchiveProject directory:
mkdir dir1 dir2 dir3.

This command creates three subdirectories: dir1, dir2, and dir3, which will be used to store the sample files.

### 3. Sample Files in Each Directory
Add sample text files to each directory:

echo "This is file1 in dir1" > dir1/file1.txt
echo "This is file2 in dir2" > dir2/file2.txt
echo "This is file3 in dir3" > dir3/file3.txt

At this point, the directory structure looks like this:
ArchiveProject/
├── dir1/
│   └── file1.txt
├── dir2/
│   └── file2.txt
└── dir3/
    └── file3.txt

### 4. Archive the Directories
Navigate to the parent directory and create an archive:

cd ..
tar -cvf project_archive.tar ArchiveProject

### 5. Compress the Archive
Compress the .tar file using gzip:

gzip project_archive.tar

This will create a compressed file named project_archive.tar.gz.

### 6. Extract the Archive
To practice extraction, first create a new directory:

mkdir ExtractedArchive

Move the compressed archive into this new directory:

mv project_archive.tar.gz ExtractedArchive/
cd ExtractedArchive

### 7. Decompress and Extract
Extract the contents of the compressed archive:

tar -xzvf project_archive.tar.gz

The contents will be extracted into an ArchiveProject folder within ExtractedArchive, recreating the original directory structure.

### 8. Verify the Extraction
List the contents to verify that the files and structure match the original:

ls -R ArchiveProject

- Summary of Commands Used
- Directory and File Creation: mkdir, echo
- Archive Creation: tar -cvf
- Compression: gzip
- Decompression and Extraction: tar -xzvf