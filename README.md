# Open Models 2026

Notebooks and materials for teaching language models by running small open models right inside Jupyter.

This is the companion repo for our SIGCSE TS 2027 demo, **Teaching LLM Engineering with Tiny Open Models in Jupyter - Cloudbank Classroom** (Sacramento, February 17-20, 2027).

## The idea

Most students meet a language model through a chat app or a commercial API, so the model stays invisible. Here the model is just another object in your notebook. You load it, see the exact chat template it receives, change the system prompt, turn the generation knobs, and test what comes back with a few lines of Python.

## The notebooks

Each one stands on its own, so you can start anywhere.

| # | Notebook | What you do |
|---|---|---|
| 1 | [Run the model](notebooks/01-run-the-model.ipynb) | Load a small model with llama-cpp-python and call it from Python. Try `max_tokens`, `temperature`, a system message, few-shot examples, and see why the chat format matters. |
| 2 | [Prompts and context](notebooks/02-prompts-and-context.ipynb) | Why the model does not remember anything, how the messages list works, dynamic system prompts for different students, and keeping the history from getting too long. |
| 3 | [Generation settings](notebooks/03-generation-settings.ipynb) | Temperature, tokens, few-shot, hallucination and sycophancy, then build a writing assistant with a system prompt. |
| 4 | [Evaluation](notebooks/04-evaluation.ipynb) | Have the model take open SAT-style questions, pull its answers out with Python, and score it on a whole set instead of one answer at a time. |
| 5 | [AI tutor](notebooks/05-ai-tutor.ipynb) | Build a course tutor: load course materials, search them, and have the model answer from what it found (RAG). |

**Extras:** [Tokens and weights](notebooks/extras/tokens-and-weights.ipynb) opens up a GGUF file to show the tokens, the vocabulary, and the weights as plain numbers.

**For instructors:** [Download models](instructor/download-models.ipynb) puts GGUF models in a shared folder for the whole class. [GPU explorer](instructor/gpu-explorer.ipynb) shows how GPU layers, threads, and context size change speed and GPU memory.

## Models and hardware

We use small open-weight models from about **0.1 to 8 billion parameters**.

- Many activities run on **CPU**.
- The larger models run on a **shared classroom GPU** (NVIDIA T4, 16 GB). An 8B model at 4-bit is about 5 GB, so two students sharing one T4 both fit.

## Running it

You can run these on any JupyterHub or on your own laptop. No commercial API account is needed.

If you teach with [CloudBank Classroom](https://docs.classroom.cloudbank.org), the Python packages are already in the hub image, so students do not install anything.

## Where these came from

These notebooks started in [ds-modules/Small_Models_SP26](https://github.com/ds-modules/Small_Models_SP26), our Spring 2026 intro to AI materials. Each notebook keeps its original authors.

## License

BSD 3-Clause. Use it, change it, and teach with it.
