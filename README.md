# auto files cluster

This is a simple Bash script that organizes files in a given folder by their file types (based on their extensions). It moves each file into a new folder named after its extension.

## Features
- Automatically creates folders based on file extensions
- Moves files into their corresponding type folders
- Helps keep directories clean and organized

## Usage
```bash
./cluster_files.sh <folder_path>
```

### Example
```bash
./cluster_files.sh /home/user/Downloads
```

If the `Downloads` folder contains files like `file.txt`, `image.png`, and `document.pdf`, the script will create the following structure:
```
Downloads/
├── txt/
│   └── file.txt
├── png/
│   └── image.png
└── pdf/
    └── document.pdf
```

## Requirements
- Bash (Linux/macOS)
- Execution permissions for the script

## How to Give Execution Permission
```bash
chmod +x cluster_files.sh
cluster_files.sh .
```

## Notes
- Only files in the top level of the given directory are affected.
- Hidden files and files without extensions are ignored.

