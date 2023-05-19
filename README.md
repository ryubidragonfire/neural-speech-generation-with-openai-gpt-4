# Neural Speech and OpenAI GPT-4 : 'Act' The Shakespeare's Play of *The Comedy of Horrors*

## Industry: Media and Entertainment
---
## Use Case: Using Neural Speech and OpenAI to Generate Audio for a Play.

This repo illustrates how to use 
- Azure OpenAI GPT-4 to extract entities from a play script, namely `Act`, `Scene`, `Setting`, `Character`, `Dialouge`, `Enter` and `Exit`. 
- Then, `Dialogue` are fed into Azure Text to Speech Cognitive Services to generate neural speech. 

Note:
- The code samples in this repository are experimental, and not suitable for production. 
- `voice` used in this example are from *Azure Speech Studio Voice Gallery*. For realistic quality of speech, consider *Azure Speech Studio Custom Voice*. 

## Data:
Shakespeare's Play of *The Comedy of Horrors* is in open domain. 

## Notebooks:
- [01-play-script-entities-extraction.ipynb](./notebooks/01-play-script-entities-extraction.ipynb) contains [prompt design](./data/few-shot-example.txt) and code which enable entity extractions from a play script. 

- [02-neural-speech-generation.ipynb](./notebooks/02-neural-speech-generation.ipynb) contains code that use *Azure Text to Speech Cognitive Service* to generate speech using a collection of default neural voices. 

- [03-merge-audio-files.ipynb](./notebooks/03-merge-audio-files.ipynb) contains the utility code in merging individual audio files. 

## Output
- [output/gpt/](./output/gpt/) contains outputs generated by *Azure OpenAI* `gpt-4-32k`.
- [output/audio/](./output/audio/) contains outputs generated by *Azure Text to Speech Cognitive Service*.

## Related repos from author
- https://github.com/ryubidragonfire/generate-podcast-synopsis-OpenAI-GPT
- https://github.com/ryubidragonfire/personalised-movie-reviews-gpt-3
- https://github.com/ryubidragonfire/document-analysis-using-gpt-3
- https://github.com/ryubidragonfire/code-explaination-openai
- https://github.com/Azure/azure-openai-samples
