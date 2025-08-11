# Claude Code Test Executor & Analyzer

A Claude Code agent that runs tests and analyzes results **without polluting your main conversation context**.

## Why this exists
- **Context efficiency**: Main agent stays clean - no verbose logs cluttering your conversation
- **Persistent logs**: Test output saved to files for detailed review when needed
- **Smart analysis**: Get actionable insights without drowning in raw test data

## What it does
- Executes tests using `./tests/run-with-log.sh` with full log capture
- Analyzes failures and provides concise, actionable insights
- Saves complete logs to files for your review
- Returns only the essential information to your main conversation

## Usage
```
"Run the authentication e2e tests and analyze any issues"
"The workflow tests keep failing - can you investigate?"
```

## Output
- **To conversation**: Clean summary with critical issues and fixes
- **To log files**: Complete test output for detailed debugging

Perfect for keeping your main Claude conversation focused while still getting comprehensive test analysis and keeping the raw data available.
