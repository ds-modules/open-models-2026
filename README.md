# Open Models 2026

Notebooks and materials for teaching language models by running small open models right inside Jupyter.

This is the companion repo for our SIGCSE TS 2027 demo, **Teaching LLM Engineering with Tiny Open Models in Jupyter - Cloudbank Classroom** (Sacramento, February 17-20, 2027).

## The idea

Most students meet a language model through a chat app or a commercial API, so the model stays invisible. Here the model is just another object in your notebook. You load it, see the exact chat template it receives, change the system prompt, turn the generation knobs, and test what comes back with a few lines of Python.

## The notebooks

Coming soon. Here is the plan. Each one stands on its own, so you can start anywhere.

| # | Notebook | What you do |
|---|---|---|
| 1 | Run the model | Load a small model and get a response from a few lines of Python. See exactly what goes in and what comes out. |
| 2 | Prompts and behavior | Change the system prompt and conversation history. Predict how the answers change. |
| 3 | Generation | Turn temperature and the other generation settings and watch what happens. |
| 4 | Evaluation | Build a small set of test questions and compare prompts and settings, instead of judging one answer at a time. |
| 5 | Build a tutor | Put the model, the system prompt, and some Python together into a tutor that guides a student to the answer instead of giving it away. |

## Models and hardware

We use small open-weight models from about **0.1 to 8 billion parameters**.

- Many activities run on **CPU**.
- The larger models run on a **shared classroom GPU** (NVIDIA T4, 16 GB). An 8B model at 4-bit is about 5 GB, so two students sharing one T4 both fit.

## Running it

You can run these on any JupyterHub or on your own laptop. No commercial API account is needed.

If you teach with [CloudBank Classroom](https://docs.classroom.cloudbank.org), the Python packages are already in the hub image, so students do not install anything.

## License

BSD 3-Clause. Use it, change it, and teach with it.
