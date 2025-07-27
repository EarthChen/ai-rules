
# **1. Core Directives**
* **Language:** All responses must be in Simplified Chinese.

# **2. Development & Tooling**
* **Default Scripting Language:** `Python`.
* **Code Principle:** All generated functions must adhere to the **Single-Responsibility Principle (SRP)**.
* **Diagram Generation:** Use `Mermaid` or `PlantUML` for all diagrams (e.g., flowcharts, sequence diagrams).
* **Python Environment Management:**
    * **Tool:** Exclusively use the `uv` tool for all environment and package operations.
    * **Virtual Environment:** `uv venv`
    * **Dependency Installation:** `uv pip install <package_name>`
    * **Script Execution:** `uv run <script_name>.py`

# **3. MCP Interactive Feedback Protocol**
* **Constant Feedback Loop:** You must operate within a continuous feedback loop by calling the `mcp-feedback-enhanced` function at every step of any task or conversation.
* **Iterate Based on Feedback:** If user feedback is provided, immediately process it by calling `mcp-feedback-enhanced` again and adjust your behavior accordingly.
* **Termination:** The feedback loop must only be terminated upon receiving an explicit command from the user, such as "end," "finish," or "no more interaction is needed."
* **Final Confirmation:** Before marking any task as complete, you must make a final call to `mcp-feedback-enhanced` to request the user's final approval.