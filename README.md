# AutoTranslatePPT

A simple(<100 loc) program that uses the [python-pptx](https://github.com/scanny/python-pptx) library and a LLM API to translate Powerpoint Slides from Chinese to English. 

The below example is part of the input.pptx and output.pptx files above, which used the gpt-3.5-turbo OpenAI LLM to translate.
![image](https://github.com/jhlimm8/AutoTranslatePPT/assets/103594440/8b3c0b6a-3ac1-41e4-bf8a-ef959ab3626e)
![image](https://github.com/jhlimm8/AutoTranslatePPT/assets/103594440/3cb198ff-2a0e-4a37-9829-d431b49c737f)

# quick start
This program supports integration with the APIs from OpenAI, TogetherAI, and Groq. This allows the user to choose from a range of different models at different price-to-performance ratios.

To specify the desired API provider and model, pass their names as arguments in your code.
## Using gpt 3.5 turbo via OpenAI API
```
pip install python-pptx openai
```
```
python translate.py YOUR_API_KEY_HERE input.pptx output.pptx OpenAI gpt-3.5-turbo 
```
## Using Qwen 2 72B via TogetherAI API
```
pip install python-pptx together
```
```
python translate.py YOUR_API_KEY_HERE input.pptx output.pptx TogetherAI Qwen/Qwen2-72B-Instruct
```
## Using Llama 3 70B via Groq API
```
pip install python-pptx groq
```
```
python translate.py YOUR_API_KEY_HERE input.pptx output.pptx Groq llama3-70b-8192
```
