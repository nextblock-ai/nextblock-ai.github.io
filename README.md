# Puck: An Autonmous and Extensible GPT-4 Experiment 
## built by NextBlock
[![Discord Follow](https://dcbadge.vercel.app/api/server/wCkJFveHeF?style=flat)](https://discord.gg/wCkJFveHeF)
[![Twitter Follow](https://img.shields.io/twitter/url/https/twitter.com/bukotsunikki.svg?style=social&label=Follow%20%40NextBlockAI)](https://twitter.com/nextblockai)



## 💡 Get help - [Q&A](https://github.com/nextblock-ai/nextblock-ai.github.io/discussions/1) or [Discord 💬]([https://discord.gg/wCkJFveHeF])
<hr/>

### 🔴 🔴 🔴  Urgent: USE `stable` not `master`  🔴 🔴 🔴

**Download the latest `stable` release from here: https:/.**
The `master` branch may often be in a **broken** state.

<hr/>


Puck is an experimental open-source application enhancing the capabilities of the GPT-4 language model. This infastructure provides an interface to interact with files on your system and automate them to leverage and extend GPT's capabilities. As one of the first examples of GPT-4 file interface, Puck pushes the boundaries of what is possible with AI. Made by the NextBlock team

We use Auto GPT capabilities 

## 🚀 Features

- 🌐 File Interaction with GPT4
- 💾 Self Referential Prompts
- 🧠 AI Agent and Person Plug-Ins
- 🔗 Extenisbility to other systems


<h2 align="center"> Demo Upcoming </h2>

https://media.moddb.com/cache/images/games/1/43/42826/thumb_620x2000/COMING_SOON.jpg

Demo made by <a href=https://>Team</a>

<h2 align="center"> 💖 Help Fund Pucks's Development 💖</h2>
<p align="center">
If you can spare a coffee, you can help to cover the costs of developing Puck and help push the boundaries of what is possible.
Your support is greatly appreciated
Development of this free, open-source project is made possible by all the <a href="https</a> and <a href="https:</a>. If you'd like to sponsor this project and have your avatar or company logo appear below <a href="https:/">click here</a>.
</p>

<p align="center">

<p align="center">

# Table of Contents

- [Installation](#installation)
- [User Guide](#userguide)
- [Functionality](#functionality)
- [Troubleshooting](#troubleshooting)
- [License and Limitations](#license)


  Team Based Interactions.... Answer each other's questions...
  
  
  # 📋 Installation
  
  ## 📋 Requirements

      - Environment (pick one)
       - [VSCode + devcontainer](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers): It has been configured in the       .devcontainer folder and can be used directly
     - Docker
     - Python 3.10 or later (instructions: [for Windows](https://www.tutorialspoint.com/how-to-install-python-in-windows))
     - [OpenAI API key](https://platform.openai.com/account/api-keys)


  ## 💾 Install


    Before installing Puck, ensure that you have [Node.js](https://nodejs.org/en/) installed on your system.

      1. Clone this repository to your local machine:

            ```
            git clone https://github.com/yourusername/puck.git
            cd puck
             ```

      2. Install the required dependencies:

            ```
             npm install
             ```

      3. Set up your OpenAI API key by creating a `.env` file in the same directory as the script and adding the following line:

             ```
             OPENAI_KEY=your_openai_api_key_here
             ```

           ** Replace `your_openai_api_key_here` with your actual OpenAI API key.**

      4. Run Puck using the following command:

             ```
             npm start
             ```
   
  ## ⚠️ OpenAI API Keys Configuration ⚠️ 

      Obtain your OpenAI API key from: https://platform.openai.com/account/api-keys.

      To use OpenAI API key for Puck, you **NEED** to have billing set up (AKA paid account).

      You can set up paid account at https://platform.openai.com/account/billing/overview.

      ![For OpenAI API key to work, set up paid account at OpenAI API > Billing](./docs/imgs/openai-api-key-billing-paid-account.png)

      #### **PLEASE ENSURE YOU HAVE DONE THIS STEP BEFORE PROCEEDING, OTHERWISE NOTHING WILL WORK!**

  
  
  
# 🗺️ User Guide
  
  
  ### Initial Workflow
  
  
  ### Advanced WOrkflow
  
  
  ### Best Practices 
  
  
  ### Prompt Examples
  
  
  
  

# 🔧Functionality

  ##What can you do with Puck?

    Here's a list of tasks and capabilities that Puck offers to showcase its power and flexibility:

    1. **File management**: Puck can handle various file-related operations like creating, moving, renaming, and deleting files and directories.
    2. **System information**: Retrieve information about the system, such as hardware details, available resources, and running processes.
    3. **Text processing**: Puck can generate and manipulate text, including searching, filtering, and modifying files or output from other commands.
    4. **Network management**: Perform network diagnostics and tasks, such as checking connectivity, monitoring network traffic, and configuring network         settings.
    5. **Software management**: Manage software packages, including installation, removal, and updates.
    6. **User management**: Create, modify, and delete user accounts, as well as manage permissions and groups on the system.
    7. **Task automation**: Automate repetitive tasks by generating scripts or combining multiple commands into a single, more efficient command.
    8. **Code generation**: Generate example code snippets or templates based on user input for various programming languages.
    9. **Troubleshooting**: Diagnose and fix common issues with the system or provide guidance on how to resolve problems.
    10. **Custom command creation**: Create custom commands or aliases for frequently used or complex commands to streamline the user experience.

    It's worth mentioning that Puck's capabilities are limited only by the power of the OpenAI API and the user's imagination. Users can leverage Puck        to interact with their system through natural language, making complex shell operations more accessible and user-friendly.

  ## Examples
  
  Here's an example of a complex task that Puck can potentially solve:

    **Task**: Compare the contents of two directories, generate a report on the differences, and email it.

    To accomplish this task using Puck, you would provide a natural language query, like:

      ```
      Compare the contents of directory1 and directory2, generate a report highlighting the differences, and email the report to example@example.com.
      ```

    Based on this input, Puck can generate and execute a series of shell commands to perform the task as described:

1. Use the `diff` command to compare the contents of the two directories and output the differences to a file named `difference_report.txt`:

   ```
   diff -r directory1 directory2 > difference_report.txt
   ```

2. Install a command-line email client like `mutt`, if it's not already installed:

   ```
   sudo apt-get install mutt
   ```

3. Send the generated report `difference_report.txt` as an email attachment to the specified email address:

   ```
   mutt -s "Directory Comparison Report" example@example.com -a difference_report.txt < /dev/null
   ```

Puck simplifies the process by allowing users to express their intent in plain language and automating the underlying shell commands. Keep in mind that the generated commands might vary depending on the user's input, system configuration, and the OpenAI API's response.


### Modes

Puck has two primary modes of operation:

1. **Execution mode**: In this mode, Puck generates and executes shell commands based on user input. To toggle execution mode, enter `$` or run Puck with the `--exec` flag:

   ```
   puck --exec
   ```

2. **View-only mode**: In this mode, Puck generates shell commands but does not execute them. This is useful for reviewing and verifying commands before running them. To toggle view-only mode, enter `.` or run Puck with the `--view` flag:

   ```
   puck --view
   ```



### Logs


### Docker


### Commands

Puck supports a number of built-in commands for managing and interacting with the shell:

- `help [topic]`: Display help information for a specific topic.
- `$<command>`: Execute a shell command.
- `puck <query1> ... <queryn>`: Recursively execute queries with Puck.
- `+ <file>`: Run a file of commands.
- `!`: Toggle hands-free (autonomous) mode.
- `push`: Push message(s) to the conversation.
- `pop`: Pop n messages from the conversation.
- `ask`: Ask the user a question.
- `done`: End the conversation.

### Aliases

Puck allows you to create and manage command aliases for frequently used or complex commands. You can perform the following actions with aliases:

- `alias-add <alias> <command>`: Add a new alias.
- `alias-remove <alias>`: Remove an existing alias.
- `alias-update <alias> <command>`: Update an existing alias.
- `alias-list`: Display a list of all aliases.


## 🔍 Google API Keys Configuration

This section is optional, use the official google api if you are having issues with error 429 when running a google search.
To use the `google_official_search` command, you need to set up your Google API keys in your environment variables.

1. Go to the [Google Cloud Console](https://console.cloud.google.com/).
2. If you don't already have an account, create one and log in.
3. Create a new project by clicking on the "Select a Project" dropdown at the top of the page and clicking "New Project". Give it a name and click "Create".
4. Go to the [APIs & Services Dashboard](https://console.cloud.google.com/apis/dashboard) and click "Enable APIs and Services". Search for "Custom Search API" and click on it, then click "Enable".
5. Go to the [Credentials](https://console.cloud.google.com/apis/credentials) page and click "Create Credentials". Choose "API Key".
6. Copy the API key and set it as an environment variable named `GOOGLE_API_KEY` on your machine. See setting up environment variables below.
7. [Enable](https://console.developers.google.com/apis/api/customsearch.googleapis.com) the Custom Search API on your project. (Might need to wait few minutes to propagate)
8. Go to the [Custom Search Engine](https://cse.google.com/cse/all) page and click "Add".
9. Set up your search engine by following the prompts. You can choose to search the entire web or specific sites.
10. Once you've created your search engine, click on "Control Panel" and then "Basics". Copy the "Search engine ID" and set it as an environment variable named `CUSTOM_SEARCH_ENGINE_ID` on your machine. See setting up environment variables below.

_Remember that your free daily custom search quota allows only up to 100 searches. To increase this limit, you need to assign a billing account to the project to profit from up to 10K daily searches._

  # License

Puck is released under the [MIT License](https://opensource.org/licenses/MIT).# Design an application


## ⚠️ Limitations

This experiment aims to showcase the potential of GPT-4 but comes with some limitations:

1. Not a polished application or product, just an experiment
2. May not perform well in complex, real-world business scenarios. In fact, if it actually does, please share your results!
3. Quite expensive to run, so set and monitor your API key limits with OpenAI!

## 🛡 Disclaimer

Disclaimer
This project, Puck, is an experimental application and is provided "as-is" without any warranty, express or implied. By using this software, you agree to assume all risks associated with its use, including but not limited to data loss, system failure, or any other issues that may arise.

The developers and contributors of this project do not accept any responsibility or liability for any losses, damages, or other consequences that may occur as a result of using this software. You are solely responsible for any decisions and actions taken based on the information provided by Puc.

**Please note that the use of the GPT-4 language model can be expensive due to its token usage.** By utilizing this project, you acknowledge that you are responsible for monitoring and managing your own token usage and the associated costs. It is highly recommended to check your OpenAI API usage regularly and set up any necessary limits or alerts to prevent unexpected charges.

As an experiment with access to your files, Puck may generate content or take actions that are not in line with real-world business practices or legal requirements. It is your responsibility to ensure that any actions or decisions made based on the output of this software comply with all applicable laws, regulations, and ethical standards. The developers and contributors of this project shall not be held responsible for any consequences arising from the use of this software.

By using Puck, you agree to indemnify, defend, and hold harmless the developers, contributors, and any affiliated parties from and against any and all claims, damages, losses, liabilities, costs, and expenses (including reasonable attorneys' fees) arising from your use of this software or your violation of these terms.

## 🐦 Connect with Us on Twitter

Stay up-to-date with the latest news, updates, and insights about Puck by following our Twitter accounts. Engage with the developer and the AI's own account for interesting discussions, project updates, and more.

- **Developer**: Follow [@NextBlock.ai](https://twitter.com/) for insights into the development process, project updates, and related topics from the creator of Puck.
- **Puck**: Join the conversation with the AI itself by following [@](https://twitter.com/nextblock). Share your experiences, discuss the AI's outputs, and engage with the growing community of users.


<p align="center">
  <a href="https:">
    <img src="https:e" alt="">
  </a>
</p>

## Run tests

To run all tests, run the following command:

# Troubleshooting

If you encounter issues while using Puck, please ensure that you have installed all the necessary dependencies and have set up your OpenAI API key correctly. If the problem persists, provide any error messages or a detailed description of the unexpected behavior so that we can better assist you.

  ## Common Problems
  
  ## Common Solutions
  
  ## FAQ
  

