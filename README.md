<p>
<a href="https://discord.gg/yjEgCgvefr"><img alt="Discord" src="https://img.shields.io/discord/1111357170504699954"></a>
</p>


<img width="1445" alt="image" style="border-radius:20px" src="https://github.com/openchatai/OpenCopilot/assets/32633162/340d174b-6ddd-452f-a66d-6c5567cc4583">


**Documentation [available here](https://docs.opencopilot.so)**

------
# 🔥 OpenCopilot

---- 
OpenCopilot allows you to have your own product's AI copilot. It integrates with your underlying APIs and can execute API calls whenever needed. It uses LLMs to determine if the user's request requires calling an API endpoint. Then, it decides which endpoint to call and passes the appropriate payload based on the given API definition.

## How does it work?
- Provide your API/backend definition, including your public endpoints and how to call them. Currently, OpenCopilot supports Swagger OpenAPI 3.0. We're also working on a UI to allow you to dynamically add endpoints.
- OpenCopilot validates your schema to achieve the best results.
- We feed the API definition to an LLM.
- Finally, you can integrate our user-friendly chat bubble into your SaaS app.



(In this example, the user was able to add a new fish to the store just by text commands)



## 🚀 Getting Started

- Make sure you have docker installed. 

- To begin, clone this Git repository:

```
git clone git@github.com:openchatai/OpenCopilot.git
```

Please find below an update concerning the API key configuration in our system.

In the `.env` file located in the `llm-server` directory, make sure to replace the placeholder value for the `OPENAI_API_KEY` variable with your actual token:

```
OPENAI_API_KEY=YOUR_TOKEN_HERE
MYSQL_URI=mysql+pymysql://dbuser:dbpass@mysql:3306/opencopilot
QDRANT_PASS=bW9tZW50bmVhcmZld2VyYXJ0YmVuZG1pbGticmVhdGhldGFsZXN3aGFsZW5vYm9keXM=
```

Regarding the `QDRANT_PASS` variable, be advised that the current value functions as the default API key for Qdrant. We highly recommend customizing this key to suit your needs by modifying the corresponding value within the `qdrant_config.yaml` file.

### For Linux Machines

To install the necessary dependencies and set up the environment for the OpenCopilot project, use the following command:

```bash
make install
```

### For ARM Machines (Mac Silicon)

If you are using an ARM machine, specifically Mac Silicon, use the following command to install dependencies and set up the environment:

```bash
make install-arm
```

Once the installation is complete, you can access the OpenCopilot console at [http://localhost:8888](http://localhost:8888).

## Additional Commands

- **make migrate**: Run Alembic migrations.
- **make down**: Stop and remove all containers.
- **make exec-dashboard**: Access the dashboard container's shell.
- **make exec-llm-server**: Access the llm-server container's shell.
- **make restart**: Restart all containers.
- **make logs**: Show container logs.
- **make purge**: Fully clean uninstall (remove containers, networks, volumes, .env).
- **make help**: Display help message with available targets.


This will install the necessary dependencies and set up the environment for the OpenCopilot project.

Once the installation is complete, you can access the OpenCopilot console at http://localhost:8888



## Try it out:
**You can try it out on [opencopilot.so](http://opencopilot.so/)**



[![IMAGE ALT TEXT](https://github.com/openchatai/OpenCopilot/assets/32633162/edebbaa6-eba5-4f72-b88d-cf0d690fffa8)](http://www.youtube.com/watch?v=HVvbY7A7lIQ "Video Title")


(OpenCopilot is not affiliated with Shopify, and they do not use OpenCopilot, it's just a demo of what copilots are capable of)


## AI Copilot: a growing trend

- [Shopify is developing "Shopify Sidekick."](https://www.youtube.com/watch?v=HVvbY7A7lIQ&ab_channel=Shopify)
- [Microsoft is working on "Windows Copilot."](https://www.youtube.com/watch?v=FCfwc-NNo30&ab_channel=MicrosoftDeveloper)
- [GitHub is in the process of creating "GitHub Copilot."](https://github.com/features/copilot)
- [Microsoft is also developing "Bing Copilot."](https://www.microsoft.com/en-us/bing?form=MA13FV)


Our goal is to empower every SaaS product with the ability to have their own AI copilots tailored for their unique products.

## 🏁 What OpenCopilot can and can't do now?

- It is capable of calling your underlying APIs.
- It can transform the response into meaningful text.
- It can automatically populate certain request payload fields based on the context.
  - For instance, you can request actions like: "Initiate a new case about X problem," and the title field will be automatically filled with the appropriate name.
- It is not suitable for handling large APIs (you will need to write JSON transformers to make it work, refer to the docs for more)



## 🛣️ Teach the copilot via flows:
Most of the time, the copilot can figure out what actions to execute when the user requests something, but in case there is a complex flow, you can define it to help the copilot:

<img width="1453" alt="image 2" src="https://github.com/openchatai/OpenCopilot/assets/32633162/81cb899c-0200-40c6-bc2f-4fe49e112085">



## 🛣️ Embed on your app in a few lines of code
Less than <10 lines of codes to implement on your web app or desktop app

<img width="1445" alt="image" src="https://github.com/openchatai/OpenCopilot/assets/32633162/d2ad2597-9de2-4177-b894-7ce92dfd1fcd">





### Important links
- [OpenCopilot Flows Editor](https://editor.opencopilot.so)
- The backend server (API) is reachable via http://localhost:8888/backend
- The dashboard server is reachable via http://localhost:8888/ or http://localhost:8888/dashboard
 

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind are welcome!



## Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind are welcome!

We love hearing from you! Got any cool ideas or requests? We're all ears! So, if you have something in mind, give us a shout! 

