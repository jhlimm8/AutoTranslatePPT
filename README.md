# AutoTranslatePPT

A simple(<100 loc) program that uses the [python-pptx](https://github.com/scanny/python-pptx) library and a LLM API to translate Powerpoint Slides from Chinese to English. 

The below example images are part of the input.pptx and output.pptx files above, which used the gpt-4o LLM to translate.
<>
# quick start
The program has integration for the OpenAI, TogetherAI, and Groq APIs. One can choose between the performant but relatively pricey gpt-4o LLM, or the slightly less performant but significantly cheaper Qwen-72B LLM, by passing the name of the desired API provider and model in the args.
## Using OpenAI API
```
pip install python-pptx openai
```
```
python translate.py YOUR_API_KEY_HERE input.pptx output.pptx OpenAI gpt-4o 
```
## Using TogetherAI API
```
pip install python-pptx together
```
```
python translate.py YOUR_API_KEY_HERE input.pptx output.pptx TogetherAI Qwen/Qwen2-72B-Instruct
```
## Using Groq API
```
pip install python-pptx groq
```
```
python translate.py YOUR_API_KEY_HERE input.pptx output.pptx Groq llama3-70b-8192
```
