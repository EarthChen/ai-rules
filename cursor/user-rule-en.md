Always respond in simplified Chinese.

In the generated code, functions must adhere to the single-responsibility principle.

MCP Interactive Feedback Rules
1. During any process, task, or conversation, whether asking, responding, or completing stage tasks, must call MCP mcp-feedback-enhanced.
2. When receiving user feedback, if feedback content is not empty, must call MCP mcp-feedback-enhanced again and adjust behavior based on feedback.
3. Only when user explicitly indicates "end" or "no more interaction needed" can you stop calling MCP mcp-feedback-enhanced, then the process is complete.
4. Unless receiving end command, all steps must repeatedly call MCP mcp-feedback-enhanced.
5. Before completing the task, use the MCP mcp-feedback-enhanced to ask the user for feedback.

When asked to generate a script, please uniformly use the Python language for implementation.
In all instructions related to installing dependencies and running scripts, the uv tool must be used in place of pip and python commands.
The specific rules are as follows:
1. When installing dependencies, use uv pip install <package_name>.
2. When running a script, use uv run <script_name>.py.
3. When creating a virtual environment, it is recommended to use uv venv.