# Discussion

## Solutions Considered
- **Reading Entire File into Memory**: This approach was discarded due to memory constraints, especially with a file size of 1 TB.
- **Using a Database**: While a database could provide efficient querying, it would require additional setup and complexity for this task.
- **Line-by-Line Reading**: This is the chosen approach as it is memory efficient and allows processing of large files without loading them entirely into memory.

## Final Solution Summary
The final solution involves reading the log file line by line to extract entries for a specific date. This method is efficient in terms of both time and memory usage, making it suitable for handling large log files.

## Steps to Run
1. Ensure you have Node.js installed on your machine.
2. Clone the repository to your local machine.
3. Create a file named `test_logs.log` in the root directory and populate it with log entries.
4. Run the script using the command:
   ```bash
   node extract_logs.js YYYY-MM-DD