# C# Tech Challenge

## Welcome!

We're excited for you to tackle this C# coding challenge! It's designed to give us a glimpse into your technical skills and how you approach problem-solving.

## Your Task (Estimated Time: ~4 hours)

You'll be building a service that processes a log file (`logs/webrtc_studio.log`), provides a simple Web API, and includes unit tests.

### Here's a quick rundown:

1. **Log Parsing**: Extract key data from the provided log file (timestamps, event types, user IDs, etc.).
2. **Data Aggregation**: Calculate user activity (joins/leaves) and error counts.
3. **Web API**: Create a Core Minimal API endpoint (`/api/loganalysis`) to serve the aggregated data in JSON format (example JSON structure provided below).
4. **Unit Testing**: Write tests to ensure your solution is robust.

### Example JSON Response:

```json
{
    "totalUserJoins": 4,
    "totalUserLeaves": 4,
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
    }
}
```

## Submission & Timeline

Thank you for your interest in our fullstack developer role. As part of our screening process, we invite you to complete the following technical exercise and submit your solution within 5 days of receiving these instructions.

### To submit your solution:

* Clone this repository to your local machine.
* Create a new public repository on your own GitHub account. Please name this repository clearly, for example: [YourGitHubUsername]-log-analysis.
* Copy the required files from the cloned version of this repository into the main branch of your newly created public repository.
* Develop your solution in a feature branch within your new public repository, ensuring you address all the requirements of the test.
* Once you have completed the exercise within the 5-day timeframe, create a pull request from your feature branch to the main branch of your own public repository.
* In the description of this pull request (the one in your repository), please tag @livener-dev. This will notify our team to review your submission.
* Ensure your repository includes a clear README file with instructions on how to run your application and any associated tests.
* Use descriptive commit messages throughout your development process in your feature branch.
* Clearly outline key features, approaches, review instructions, and trade-offs in your pull request description.


## Evaluation

### We'll be looking at:

* **Correctness:** How accurately your code parses the log and aggregates the data.
* **Code Quality:** Readability and maintainability.
* **Testing:** How well you've covered key functionality with unit tests.
* **Web API:** Functionality and JSON structure.

**Note:** A working solution is required to proceed to the in person part of our interview.

To ensure a smooth transition to the second part of the interview, please pay close attention to the `/api/loganalysis` endpoint. Your working solution here is essential for the next steps. Please double-check that it's functioning as expected!

## Running Your Service

Please provide instructions on how to run your application locally (e.g., commands, dependencies).

## Log File & Format

The log file (`webrtc_studio.log`) and a sample log file (`SAMPLE_LOG.md`) with the format details are located in the `/logs` directory.

## We're Excited!

We're excited to see your solution! Good luck!
