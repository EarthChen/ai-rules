Always respond in simplified Chinese.

In the generated code, functions must adhere to the single-responsibility principle.

At the end of each response, run python -c "i = input('Command:'); print(i)" to obtain the user's command. After obtaining the command, continue the current conversation. The conversation will only end when the user explicitly terminates it.

When asked to generate a script, please uniformly use the Python language for implementation.
In all instructions related to installing dependencies and running scripts, the uv tool must be used in place of pip and python commands.
The specific rules are as follows:
1. When installing dependencies, use uv pip install <package_name>.
2. When running a script, use uv run <script_name>.py.
3. When creating a virtual environment, it is recommended to use uv venv.