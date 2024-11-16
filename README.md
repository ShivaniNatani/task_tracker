# Task Tracker CLI

## Detailed Code Explanation

The **Task Tracker CLI** is a Python script that allows users to manage their tasks from the command line. The code interacts with a `tasks.json` file that stores the tasks and their attributes.

### Key Components

1. **File Handling**:  
   The script uses the `json` module to read from and write to the `tasks.json` file, which stores all tasks. If the file does not exist, it will be created with an empty list.

2. **Task Management**:  
   Tasks have several attributes, including:
   - **ID**: A unique identifier for the task.
   - **Description**: A short description of the task.
   - **Status**: The current status of the task (e.g., `todo`, `in-progress`, `done`).
   - **CreatedAt**: The timestamp when the task was created.
   - **UpdatedAt**: The timestamp when the task was last updated.
   - **DueDate**: The date the task is due.
   - **Priority**: The importance of the task (`low`, `medium`, `high`).

3. **Functions**:
   - **add_task()**: Adds a new task with description, due date, and priority.
   - **list_by_status()**: Lists tasks filtered by their status.
   - **list_by_date()**: Lists tasks filtered by created or due date.
   - **list_by_priority()**: Lists tasks filtered by priority.
   - **update_task()**: Updates the description of a task.
   - **delete_task()**: Deletes a task by its ID.
   - **mark_task()**: Marks a task as `in-progress` or `done`.

By calling these functions, users can efficiently manage their tasks, track their progress, and ensure important tasks are completed on time.
