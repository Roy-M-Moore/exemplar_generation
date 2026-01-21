# LLM-Generated Exemplars for Performance Levels

This repository contains Python scripts used to generate textual exemplar responses at predefined performance levels using the OpenAI API.

---

## Overview

For each input question, the scripts:
1. Read a system prompt and a performance-level–specific prompt
2. Combine the prompt with the input question
3. Call the OpenAI Chat Completions API
4. Save the generated exemplar text to an output file

Exemplars are generated separately for each target performance level.

---

## Performance Levels

Exemplars were generated for four target scores:
- **30/100** – poor
- **50/100** – sufficient
- **70/100** – good
- **90/100** – excellent

Each performance level corresponds to a prompt file in the `prompts/` directory.

---

## Directory Structure

- inputs/ # One .txt file per question
- prompts/ # System prompt and user prompts (one per performance-level)
- outputs/ # Generated exemplar responses

---

## Model and Generation Details

- Model: **GPT-5.1** (adjust based on requirements)
- API: OpenAI Python API
- Each exemplar is generated in a separate API call
- Prompts include the question, grading rubric, and explicit instructions to generate a response consistent with a specified target score

---

## Notes

- This repository is intended for research and reproducibility purposes.

---

## License

The repository is licensed under the MIT License.  

