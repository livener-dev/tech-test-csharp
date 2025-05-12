
# C# Tech Challenge

## Welcome!

We're excited for you to tackle this C# coding challenge! It’s designed to give us a quick glimpse into your technical skills, and how you approach problem-solving.

## Your Task (Estimated Time: **1–2 hours**)

You’ll build a small service that processes a log file (`logs/webrtc_studio.log`) and exposes a simple Web API to return structured user activity data.

### What to Build

1. **Log Processing**: Read and extract relevant data from the provided log file (e.g., timestamps, event types, user IDs).
2. **Data Aggregation**:
   - Return a list of all user activity events (JOIN/LEAVE with timestamp and userId).
   - Calculate the **total number of unique users** who joined the call.
3. **Web API**: Create a minimal API endpoint (`/api/loganalysis`) that returns the aggregated data in JSON format (see example below).
4. **(Optional Stretch Goal)**: Extend your solution to also extract and count error messages by severity level (e.g., `ERROR`, `CRITICAL`, `WARNING`) and include them in the response.

### Example JSON Response

```
{
    "uniqueUsers": 3,
    "userActivity": [
        {
            "userId": "456",
            "event": "JOIN",
            "timestamp": "2023-10-27 10:01:00"
        }
        // ... more user activity events
    ],
    "errors": {
        "ERROR": 4,
        "CRITICAL": 2,
        "WARNING": 3
    } // Optional: Only included if stretch goal is implemented
}
```

## Submission & Timeline

We’re excited to see what you build! Please follow the steps below to submit your solution.

### How to Submit

* Clone this repository to your local machine.
* In your GitHub account, create a new public repository for this project (e.g., [your-github-username]-log-analysis).
* Copy any necessary files from this repo into your new one.
* Develop your solution in a feature branch of your repository.
* Include a README.md file in your repository with clear instructions on how to run your application from the CLI.
* When you're done, open a pull request from your feature branch into the main branch of your repo.
* In your pull request description, please include:
  1. Any assumptions, design decisions, or trade-offs you made.
  2. Key features and approaches you took.
  3. Clear testing and review instructions.
* ✅ Once submitted, please email us a link to your pull request.
* 📌 You can also tag @livener-dev in the pull request description to notify our team directly.
* ⏱️ Please ensure your submission is completed within the agreed time frame.

## Evaluation

### We'll be looking at:

* **Correctness:** How accurately your code parses the log and aggregates the data.
* **Code Quality:** Readability and maintainability.
* **Testing:** How well you've covered key functionality with unit tests.
* **Web API:** Functionality and JSON structure.

**Note:** A working solution is required to proceed to the in-person stage of the interview.

To ensure a smooth transition to the second part of the interview, please pay close attention to the `/api/loganalysis` endpoint. Your working solution here is essential for the next steps. Please double-check that it's functioning as expected!

## Running Your Service

Please provide instructions on how to run your application locally (e.g., commands, dependencies).

## Log File & Format

The log file (`webrtc_studio.log`) and a sample log file (`SAMPLE_LOG.md`) with the format details are located in the `/logs` directory.

## We're Excited!

We're excited to see your solution! Good luck!
