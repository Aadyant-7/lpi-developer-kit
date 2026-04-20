## HOW I DID IT - Yash Vardhan

For Level 3, I chose Track A: Agent Builders.

First, I created a separate GitHub repository named `lpi-agent-yash` for my Level 3 project.

Then I created an `agent.py` file and started building a Python-based agent.

At first, I tried to connect to the LPI tools using `requests` and localhost, but I got connection errors because the server was not running the way I expected.

After debugging the issue, I changed the approach and used Python `subprocess` to run the LPI sandbox commands from the `lpi-developer-kit` folder.

I also fixed the folder path problem so the script could correctly run `npm run test-client` from the right location.

After that, the agent successfully returned LPI sandbox output and showed the sources used: `query_knowledge` and `get_case_studies`.

Through this process, I learned how tool-based AI agents work, how to debug connection and path problems, and how to integrate Python with command-line tools in a practical project.
