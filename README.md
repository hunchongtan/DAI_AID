# [AID Project 2] Modular AI-powered Workflow for Identification of Design Opportunities
<br/>
<p align="center">
  <img src=https://img.shields.io/badge/python-3.8%20%7C%203.9-blue.svg alt="Python Versions"/>
</p>

## Description
As part of SUTD DAI pillar's 60.002 AI applications in Design module, we are tasked to identify opportunities for design improvements. We are assigned to use data-driven text analytics and/or image processing to identify design opportunities. We are advised to focus on a specific product and conduct benchmarking with competitors whenever appropriate.
Our end result is a **series of Jupyter notebooks with a clear AI workflow for Identification of Design Opportunities**.
The clear design workflow is as such:
1. Initial Text Query with ChatGPT
2. Initial Image Contextual Query with ChatGPT
3. Data Collection and Pre-processing
4. Finding Top Words for Data Analysis
5. Identification of Design Opportunities with Classified Sentiment Analysis
6. Design Justification with Design Structure Matrix
The notebooks are meant to be modular and replicable for any product of the user's choice.

## Setup Guide

### Installation
Step 1: Clone the repo
```
git clone https://github.com/hunchongtan/DAI_AID.git
```

Step 2: Set up the  ```.env``` file by cloning the  ```.env.example``` file
```
cp .env.example .env
```

Step 3: Retrieve the following API keys from the following websites:

`OPENAI_API_KEY`:
1. Sign in to OpenAI and go to https://platform.openai.com/docs/overview
2. Expand the left panel (below the OpenAI logo) > Click on API keys > Click on + Create new secret key
3. Fill out the required details: *(refer to the first/left picture)* \
Name: any_name_for_your_app > Click on Create secret key
4. Copy the API Key as OPENAI_API_KEY *(refer to the second/right picture)*
<img src="https://github.com/hunchongtan/DAI_AID/assets/87000020/881bc85b-9e9a-4521-8cf5-b669ff99378b" height="150" />
<img src="https://github.com/hunchongtan/DAI_AID/assets/87000020/79baacd2-2c2c-4b3b-b55f-abccfd78baf6" height="150" />
<br>
<br>

`GOOGLE_API_KEY`:
1. Sign in to Google and go to https://console.cloud.google.com/
2. Expand the left panel > Click on APIs & Services > Click on Enabled APIs & services > CREATE PROJECT
3. Fill out the required details: *(refer to the first/left picture)* \
Project name: any_name_for_your_app > CREATE
4. Expand the left panel again > Click on Enabled APIs & services > Click on ENABLE APIS AND SERVICES (on top) > Scroll down and click on YouTube Data API v3
5. Click on Enable > CREATE CREDENTIALS (top right) > Select Public data > Click on Next
6. Copy the API Key as GOOGLE_API_KEY *(refer to the second/right picture)*
<img src="https://github.com/hunchongtan/DAI_AID/assets/87000020/92f6b2a6-ccea-4e45-81f8-cffc0a1a5f2d" height="150" />
<img src="https://github.com/hunchongtan/DAI_AID/assets/87000020/12145244-144d-451c-a2cb-513b22eea989" height="150" />
<br>
<br>

`REDDIT_API_ID`, `REDDIT_API_KEY`, `REDDIT_API_USER`, `REDDIT_API_PW`:
1. Sign in to Reddit and go to https://www.reddit.com/prefs/apps
2. Click are you a developer? create an app... / create another app… button
3. Fill out the required details: *(refer to the first/left picture)* \
Name: any_name_for_your_app, Select script, description: any_description, about url: Leave Empty, redirect url: your_socials_link & click create app
4. Copy the personal use script as REDDIT_API_ID and the secret token as REDDIT_API_KEY *(refer to the second/right picture)*
6. Copy your reddit username and password as REDDIT_API_USER and REDDIT_API_PW respectively
<img src="https://github.com/hunchongtan/DAI_AID/assets/87000020/8db914d3-f9f8-46b6-a5cc-f6dfb28475c4" height="150" />
<img src="https://github.com/hunchongtan/DAI_AID/assets/87000020/dd65e351-cd1a-4f25-87ff-b0c73b4e4719" height="150" />
<br>
<br>

### Data Selection
Working with Sample Data: \
If you wish to verify with sample data (Author was exploring for **Scoot 787**), please copy `support` and `others` in sample_data folder to the main folder.

Working with own Data: \
If you wish to try out on a different product, remember to clear all outputs in the jupyter notebooks before running all codes.

### Run the Notebooks
1. Follow the instructions in the jupyter notebooks.
2. Edit the data in all the TO DO SECTIONs.
3. Run the codes without editing in RUN AS INTENDED (DO NOT CHANGE ANYTHING.) sections.
4. Have fun learning the workflow!


## Acknowledgements
Our work is made possible with the help of Professor Edwin Koh's AID lectures and his <a href="https://arxiv.org/ftp/arxiv/papers/2312/2312.04134.pdf">research paper on LLM-generated DSMs</a>. \
Special thanks to the team behind this project:
- Delphine Sim Yingting (1006986)
- Tan Hun Chong (1006643)
- Cyan Koh Shi-An (1007230)
- Lim Sophie (1007487)
- Lim Ying Xuan (1006960)
- Tan Ze Lin (1007054)
