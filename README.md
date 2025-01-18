# AIagentToScrapeTheWeb
Simple way to set up an open source AI agent to scrape the web.

Here we will set up an agent that will be capable of scraping the web for us. All tools we will use are open source and free to use, which makes this simple solution for available to anyone. 

Tools we will use:
1) Linux Machine
1) AnythingLLM - a simple interface for a local model.
2) 


First, go to https://anythingllm.com/ and navigate to "Download for Desktop" button
![image](https://github.com/user-attachments/assets/d0232931-5c31-493e-852f-8fd5484c7ae8)

I am using Linux, so I will choose "Download for Linux"
![image](https://github.com/user-attachments/assets/9927c8f2-6b45-4b8d-8d7f-5b104286c435)

I will make it simple and use the following scripts from the instructions given for Linux
![image](https://github.com/user-attachments/assets/3b48c676-aedf-4e99-a93d-381ed4f39d98)

You can simply copy the command below, or get it from the website.

```bash
curl -fsSL https://cdn.useanything.com/latest/installer.sh | sh
```
After the command is executed, you should receive the following confirmation of installation in your terminal and AnythingLLM will be installed on your computer.
![image](https://github.com/user-attachments/assets/86b5b517-92f7-4552-a532-19d24e17655b)

As shown in the terminal above, my installation path is /home/user/AnythingLLMDesktop. I will execute the "Start" file
![image](https://github.com/user-attachments/assets/d4701c31-9e20-4978-b6a5-55106c686bc9)

Congradulations, you are half way there!

Now, lets install Ollama for model management and a model.

You can simply go to https://ollama.com/ and click "Download"

![image](https://github.com/user-attachments/assets/67e1c852-861d-4fb9-9f94-a5a4226d983b)

Once again, I will select Linux Download as i am running a Linux Machine.

![image](https://github.com/user-attachments/assets/969226a2-dbf7-496c-b994-23145027659f)

You can simply copy BASH code below or get it from the website.

```bash
curl -fsSL https://ollama.com/install.sh | sh
```

at the end of the installation, you will receive a message indicating successfull installation that will look something like below.

![image](https://github.com/user-attachments/assets/6318ea3f-1210-4e52-8f74-8a2af17710a5)

Now, let's go back to Ollama website and navigate to "Models" section. 

![image](https://github.com/user-attachments/assets/c76c4f26-98b0-48cb-9f3b-fdc5cd6efb21)

There are plenty of different model available here that you can deploy using ollama. I will use a small model for demonstration purposes, but you can branch out if you would like. Just note that larger models will require more RAM and/or VRAM. So choose something your machine can run. 

I chose llama3.1 model with 8 bln parameters that is roughtly 4.9 GB. 





