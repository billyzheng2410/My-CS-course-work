[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/billyzheng2410/My-CS-course-work/blob/main/NLPPROJECT/final_project.ipynb)
# README: How to Run This Notebook

## 1. Open the Notebook
* It is recommended to open and run this file in **Google Colab**.
* Ensure you have a stable internet connection.

## 2. Configure the Runtime Environment (Very Important)
This code loads the `meta-llama/Llama-3.1-8B` model using `transformer_lens`, so it requires **GPU** resources:
1. Click on `Runtime` in the menu bar -> `Change runtime type`.
2. Under the Hardware accelerator dropdown menu, select **T4 GPU** or a higher-tier GPU.(For stable performance please use A100 High RAM)
3. Click `Save`, and wait for the top right corner to display `Connected`.

## 3. Hugging Face Access
Because `Llama-3.1-8B` is a Gated Model:
1. You need to register an account on [Hugging Face](https://huggingface.co/).
2. Go to the `meta-llama/Llama-3.1-8B` model page and agree to the license agreement to get access.
3. Generate an Access Token (with Read permission) in your Hugging Face account settings.
4. When running the third code cell (`notebook_login()`) in this Notebook, an input box will pop up. Please paste your Token there and log in.

## 4. Run the Code
* You can run cells one by one: select a cell and press `Shift + Enter`, or click the play button (▶) on the left side of the cell.

*Note: Environment installation (like `pip install`) may take a minute or two. Please run the cells sequentially after installation.*
 The transformer_len installartion will restart the runtime automatically, and all you need to do is run the blocks below it.
