# Linux System Administration
## Objective
The objective of this project is to evaluate your proficiency in Linux system
administration. You will be required to perform tasks involving basic and moderate Linux
commands, shell scripting, text manipulation, setting up CRON jobs, monitoring systems
performance and sending email notifications.


## Basic and Moderate Linux Commands
### Task 1
Create a directory structure as follows:
```bash
/home/<your_username>/devops_project/
├── logs
├── scripts
├── reports
├── data
└── archive
```

- Create a text file named sample.txt in the logs directory with the following content:
```bash
Hello, this is a sample file.
```

- This file is used for text manipulation.
- Copy `sample.txt` to the reports directory and rename it to `sample_backup.txt`.
- List all files in the logs and reports directories.
- Use the `find` command to locate all `.txt` files in the 
  `/home/<your_username>/devops_project/` directory and its subdirectories.
- Use the `grep` command to search for the word "sample" in all `.txt` files in the
  `/home/<your_username>/devops_project/` directory.
- Compress the reports directory into a `tar.gz` file named `reports_backup.tar.gz` and move
  it to the archive directory.
- Use the `diff` command to compare `sample.txt` and `sample_backup.txt`.

### Task 2: Shell Scripting
Write a shell script `backup.sh` that:
- Takes two arguments: source directory and destination directory.
- Copies all files from the source directory to the destination directory.
- Logs the start and end time of the backup process in a file named backup.log in the logs
  directory.

Example usage: 
```bash
./backup.sh /home/<your_username>/devops_project/logs /home/<your_username>/devops_project/reports
```

Write a shell script `file_processor.sh` that:
- Takes a directory as an argument.
- Reads each `.txt` file in the directory.
- Counts the number of lines, words, and characters in each file and appends this
  information to a file named `file_summary.log` in the logs directory.

Example usage: 
```bash
./file_processor.sh /home/<your_username>/devops_project/data
```

Write a shell script housekeeping.sh that:
- Deletes all `.log` files in the `/logs` directory that are older than 7 days.
- Archives all files in the `/data` directory that are older than 30 days into a `tar.gz` file and
  moves them to the `/archive` directory.
- Logs the housekeeping activities in a file named `housekeeping.log` in the `/logs` directory.

Example usage: 
```bash
./housekeeping.sh
```

Write a shell script monitor_disk.sh that:
- Checks the disk space utilization of the `/home` directory.
- Logs the disk space usage in a file named `disk_usage.log` in the `/logs` directory.
- Sends an email notification if the disk space usage exceeds 80%.
Example usage: 
```bash
./monitor_disk.sh
```

### Task 3: Text Manipulation
Using the `sed` command: 
- Replace the word "sample" with "example" in the `sample_backup.txt` file located in the reports directory.
- Use the `awk` command to print only the second line from the `sample_backup.txt` file.
- Use the `cut` command to extract the first and second words from each line of `sample.txt`
- Save the output to a new file named `sample_cut.txt` in the `/reports` directory.
- Use the `sort` command to `sort` the contents of `sample_cut.txt` alphabetically and save
  the sorted output to a file named `sample_sorted.txt`.

### Task 4: Cron Jobs
- Schedule the `backup.sh` script to run every day at 2 AM using a CRON job.
- Schedule the `file_processor.sh` script to run every day at 3 AM.
- Schedule the `housekeeping.sh` script to run every Sunday at 4 AM.
- Schedule the `monitor_disk.sh` script to run every hour.
- Provide the CRON job entries you added to the crontab file.

### Task 5: Monitoring System Performance
Write a shell script `monitor.sh` that:
- Monitors CPU and memory usage of the system.
- Logs the CPU and memory usage to a file named `system_monitor.log` in the logs
  directory every 5 minutes.
- Sends an email notification to a specified email address if the CPU usage exceeds 80%
  or the memory usage exceeds 90%.

### Task 6: Sending Email Notifications
- Install and configure mailx (or any other mail utility) on your Linux system.
- Update the `monitor.sh` script to send an email notification with the subject "High
  CPU/Memory Usage Alert" and the content of the `system_monitor.log` file if the CPU or
  memory usage threshold is exceeded.
- Update the `monitor_disk.sh` script to send an email notification with the subject "Disk Space Alert" and the current disk usage if the disk space usage threshold is exceeded.
