# Multi_Agent_Langgraph
This project demonstrates a simple *Multi-Agent workflow* using `LangGraph`


## 🧩 Architecture
The workflow consists of two main nodes managed by a `StateGraph`:

1.  **Planner Node 📝**:
    * Receives the user's input.
    * Uses **model-llm** to break the task into 2-3 distinct steps.
    * Passes these steps to the state.

2.  **Executor Node ⚙️**:
    * Takes the list of steps from the Planner.
    * Formats and compiles them into a final execution path.
    * Returns the final output.


