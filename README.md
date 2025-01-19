# AI Agent to Scrape the Web

This guide will walk you through setting up an open-source AI agent capable of scraping the web. All tools we will use are open-source and free, making this a simple and accessible solution for anyone.

### Tools Required:
1. **Linux Machine**
2. [AnythingLLM](https://anythingllm.com/) - A simple interface for a local model.
3. [Ollama](https://ollama.com/) - A model management tool.
4. LLaMA model (for demonstration, we'll use the `llama3.1` model)

---

## **Section 1: Install AnythingLLM**

1. **Download AnythingLLM**  
   Go to [AnythingLLM's download page](https://anythingllm.com/) and click the **"Download for Desktop"** button.

![image](https://github.com/user-attachments/assets/d0232931-5c31-493e-852f-8fd5484c7ae8)

   - If you're using Linux, select **"Download for Linux"**.

![image](https://github.com/user-attachments/assets/9927c8f2-6b45-4b8d-8d7f-5b104286c435)

   - To keep it simple, I will use the following script from the instructions provided for Linux.

![image](https://github.com/user-attachments/assets/3b48c676-aedf-4e99-a93d-381ed4f39d98)

   - You can either copy the command below or obtain it directly from the website.

```bash
curl -fsSL https://cdn.useanything.com/latest/installer.sh | sh
```

   - Once the command is executed, you should see a confirmation of the installation in your terminal, indicating that AnythingLLM has been successfully installed on your computer.

![image](https://github.com/user-attachments/assets/86b5b517-92f7-4552-a532-19d24e17655b)

   - As shown in the terminal above, the installation path is /home/user/AnythingLLMDesktop. Now, I will execute the **"Start"** file.

![image](https://github.com/user-attachments/assets/d4701c31-9e20-4978-b6a5-55106c686bc9)

   - Congratulations, you're almost there!

## **Section 2: Download and Install Ollama for Managing LLM Providers**

   - Now, let's install Ollama to manage the model and its configurations.

   - Simply visit https://ollama.com/ and click **"Download"**

![image](https://github.com/user-attachments/assets/67e1c852-861d-4fb9-9f94-a5a4226d983b)

   - Once again, I will select Linux Download since I am using a Linux machine.

![image](https://github.com/user-attachments/assets/969226a2-dbf7-496c-b994-23145027659f)

   - You can either copy the BASH code below or get it directly from the website.

```bash
curl -fsSL https://ollama.com/install.sh | sh
```

   - At the end of the installation, you should see a message indicating a successful installation, similar to the one below.

![image](https://github.com/user-attachments/assets/6318ea3f-1210-4e52-8f74-8a2af17710a5)

## **Section 3: Download and Install the LLaMA Model**

   - Now, let's return to the Ollama website and navigate to the **"Models"** section.

![image](https://github.com/user-attachments/assets/c76c4f26-98b0-48cb-9f3b-fdc5cd6efb21)

   - There are many different models available here that you can deploy using Ollama. For demonstration purposes, I will use a smaller model, but feel free to explore other options. Keep in mind that larger models may require more RAM and/or VRAM, so choose one that your machine can handle.

   - I’ve chosen the **llama3.1** model with 8 billion parameters, which is approximately 4.9 GB in size.

![image](https://github.com/user-attachments/assets/102f73c7-dd73-45a6-b365-fd3d9f7131d5)

   - As always, you can either copy the command below or obtain it directly from the website.

```bash
ollama run llama3.1
```
   - When you run the command in your terminal, Ollama will download the model (if it's not already available), complete the necessary configurations, and start the model. You can interact with the model directly through your terminal if you wish. However, in the next step, we will configure AnythingLLM to work with the model instead.

![image](https://github.com/user-attachments/assets/8115458d-a50d-4321-9df9-5e73634d5c7c)

## **    Section 4: Configure AnythingLLM to Work with Ollama**

   - Now, let's return to AnythingLLM and configure it to use the Ollama model we just installed. Simply select Ollama from the list of available LLM providers, and the model should appear automatically. If you have multiple models installed, you can choose the one you want to use.

![image](https://github.com/user-attachments/assets/92d65c7b-5c8d-4c66-b66c-22a04bd5b4e8)

   - You can take a few additional steps to review details about security and Workspaces. During the process, you'll be prompted to enter a name for the workspace that will be created. Once completed, you'll have a fully functional alternative to ChatGPT running on your own computer—ready for offline use!

![image](https://github.com/user-attachments/assets/cf147152-809b-45dc-8a77-af15dd2f4729)



## **Section 5: Set Up an Agent with Internet Access**

   - Now, let's set up an agent and configure it for internet access. Go to the workspace settings and configure the agent to use the Ollama model, as shown below.

![image](https://github.com/user-attachments/assets/76f8d464-66f9-403d-a706-0a4f35e0e77e)

   - Once you’ve updated the agent settings, you can configure it further using the same button. Click the button again to configure the search engine and enable web access for the agent, as shown below.

![image](https://github.com/user-attachments/assets/036c76d4-5af5-4ec8-8a25-80a2edf6922a)

   - For the web search to function, you'll need to register a search engine with one of the providers listed. In this example, we will use the Google Search Engine provider. Click the link to register a new engine, then proceed to your Google account to create a new search engine.

![image](https://github.com/user-attachments/assets/bb522123-5134-47d9-97cd-c4e4f5b2c958)

   - You can now preview or customize the engine you just registered. Simply go to the **"Customize"** section.

![image](https://github.com/user-attachments/assets/e7e86713-16b6-45a2-be43-06325c343682)

   - In the Overview section, you'll find the **"Search Engine ID"** under the **"Basic"** tab. Copy that ID and paste it into AnythingLLM.
   - You can also find the API key under the **"Programmatic Access"** tab.

![image](https://github.com/user-attachments/assets/2662a7f8-814a-40c7-9fd0-f0fe03197eac)

   - From there, you can click **"Get a Key"** to obtain the API key.

![image](https://github.com/user-attachments/assets/b377e468-13f0-42c4-8f89-5a9e64cb9cf5)

   - Copy the API key and paste it into AnythingLLM. Then, click **"Save"** to apply the changes.

![image](https://github.com/user-attachments/assets/d656efcc-6271-41e3-ba60-9e9d88ce9d02)

   - Congratulations! You’re all set to scrape websites using the agent you just configured! Simply use **"@agent"** in the chat to initialize the agent before making your requests, and you’re good to go!
