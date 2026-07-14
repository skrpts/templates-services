# Release Notes

## v1.0.4
GH#838 — declare the network domains the svc-* service templates reference (svc-openai→api.openai.com, svc-anthropic→api.anthropic.com, svc-cohere, svc-mistral, svc-google-gemini→googleapis.com, svc-github-api, svc-linear, svc-notion, svc-slack), plus network:localhost for the local-service templates (svc-chroma/lm-studio/ollama/qdrant), in requires.permissions. Clears the "network not declared" content-quality warnings that blocked republish; unblocks the GH#837 id-alignment republish.

## v1.0.3
GH#837 — align source `manifest.id` to the catalogue-registered id `155f70b0…` (K-037 Option A: catalogue authoritative). The old source id was referenced nowhere but this manifest.

