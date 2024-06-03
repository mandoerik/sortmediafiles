## sortmediafiles
This Ansible playbook is designed to efficiently organize media files in a given directory by sorting them into a new directory structure based on their creation or modification year and month. Here's what the playbook does:

File Discovery: Scans the specified source directory to find all types of media files, including images, videos, and audio files.

Metadata Extraction: Extracts the creation or modification date for each media file.

Directory Creation: Creates a new directory structure in the destination path, organizing folders by year and subfolders by month.

If filename already exist in destination it moves the file but renames it with _1 in the destination folder..

File Sorting: Moves each media file from the source directory to its corresponding year/month folder in the destination directory.

Logging: Logs the operations performed and provides a summary report at the end.

This playbook is useful for organizing media collections, making it easier to manage and locate files based on their creation or modification dates.

```bash
ansible-playbook sortphotos.yml --extra-vars "src_dir= dest_dir="
```
