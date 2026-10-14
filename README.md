# KnowledgePilot AI

Citation-backed AI knowledge assistant with document access controls, hybrid retrieval, and a synthetic public demo.

The complete MIT-licensed source is in `knowledgepilot-ai-deploy.zip`. Extract it to inspect or run the application. Render automatically extracts the source during its build.

## Deploy

Create a Render Blueprint from this repository and supply a Groq API key as the secret `KP_LLM_API_KEY`. The service uses Render’s free plan and Groq hosted inference. Free hosting may sleep and reset demo history. Only synthetic documents are included.

## Validation

44 Python tests pass locally. Hosted API calls are mock-tested; live hosted inference must be verified after deployment. Local Qwen2.5 7B evaluation: 60 of 84 source-bearing queries accepted, with valid citation IDs on accepted answers. This is not a comprehensive human correctness evaluation.
