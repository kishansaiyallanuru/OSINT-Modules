# Day 1 – OSINT Workflow  
## Google Dorking, Search Engines & Publicly Available Resources  


## 1. Objective  

In this task, I performed Open-Source Intelligence (OSINT) using Google Dorking techniques. The goal was to understand how to refine search queries step by step and extract useful public information from the internet.


## 2. Target  

- **Primary Target:** Akhil KJ  
- **Reference Domain:** amrita.edu  



## 3. Tools Used  

- Google Search Engine  
- DuckDuckGo  
- Bing  

  

## 4. Workflow  

  

## Step 1: Performing a Normal Search  

**Query I used:**  
Akhil KJ  

**Tool I used:**  
Google  

**What I did:**  
I started with a simple search without applying any filters to see how general results appear.

**Screenshot:**  
![Step 1](Images/Step1.png)

**What I observed:**  
- I got a large number of results  
- Many results were not related to my target  
- Some results only matched part of the name (Akhil or KJ)  
- Profiles from different domains like LinkedIn, hospitals, etc., appeared  

**What I understood:**  
This search gave very broad results and included a lot of unwanted data. It showed me that normal searching is not enough for accurate OSINT.

  

## Step 2: Using Exact Match Search  

**Query I used:**  
"Akhil KJ"  

**Tool I used:**  
Google  

**What I did:**  
I used quotes to search for the exact name.

**Screenshot:**  
![Step 2](Images/Step2.png)

**What I observed:**  
- Results became more relevant  
- Exact name matches were shown  
- Irrelevant results reduced  
- Social media and specific profiles appeared  

**What I understood:**  
Using quotes helps in improving accuracy by forcing Google to match the exact phrase.

  

## Step 3: Adding Context to the Search  

**Query I used:**  
"Akhil KJ" "Amrita"  

**Tool I used:**  
Google  

**What I did:**  
I added the keyword "Amrita" to connect the person with an institution.

**Screenshot:**  
![Step 3](Images/Step3.png)

**What I observed:**  
- Results were related to Amrita Vishwa Vidyapeetham  
- Faculty profile links appeared  
- It became easier to identify the correct person  

**What I understood:**  
Adding context helps in filtering out unrelated people and improves the quality of results.

  

## Step 4: Searching Within a Specific Website  

**Query I used:**  
site:amrita.edu "Akhil KJ"  

**Tool I used:**  
Google  

**What I did:**  
I restricted the search to only the amrita.edu domain.

**Screenshot:**  
![Step 4](Images/Step4.png)

**What I observed:**  
- All results were from the official Amrita website  
- Faculty profiles and official pages appeared  
- Information looked more reliable  

**What I understood:**  
Using the `site:` operator helps in getting trusted and official information.

  

## Step 5: Finding Documents Using Filetype  

**Query I used:**  
"Akhil KJ" filetype:pdf  

**Tool I used:**  
Google  

**What I did:**  
I searched for PDF documents related to the target.

**Screenshot:**  
![Step 5](Images/Step5.png)

**What I observed:**  
- PDF documents like lists, reports, and academic files appeared  
- Some documents contained structured information  
- Useful details were available inside these files  

**What I understood:**  
Filetype search helps in finding hidden or less visible data in documents.

  

## Step 6: Discovering Email Information  

**Query I used:**  
site:amrita.edu "@amrita.edu"  

**Tool I used:**  
Google  

**What I did:**  
I searched for email addresses within the domain.

**Screenshot:**  
![Step 6](Images/Step6.png)

**What I observed:**  
- Multiple email IDs were visible  
- A common email format was identified  
- Contact-related pages appeared  

**What I understood:**  
This helps in understanding how email structures work in an organization.

  

## Step 7: Using Multiple Keywords  

**Query I used:**  
"Akhil KJ" "Amrita" "Cyber Security"  

**Tool I used:**  
Google  

**What I did:**  
I combined multiple keywords to make the search more specific.

**Screenshot:**  
![Step 7](Images/Step7.png)

**What I observed:**  
- Results were highly specific  
- Cyber Security-related profiles appeared  
- Very few irrelevant results  

**What I understood:**  
Combining multiple keywords gives very accurate and targeted results.

  

## Step 8: Using Alternative Search Engines  

**Tools I used:**  
- DuckDuckGo  
- Bing  

**What I did:**  
I repeated similar searches in other search engines.

**Screenshots:**  
![DuckDuckGo](Images/Step8_1.png)  
Using DuckDuckGo
![Bing](Images/Step8_2.png)
Bing

**What I observed:**  
- Results were slightly different from Google  
- Some unique links were found  
- DuckDuckGo showed fewer personalized results  

**What I understood:**  
Using multiple search engines helps in getting better coverage and finding additional information.

  

## 5. Conclusion  

From this task, I understood that simple searching is not enough for OSINT. By applying Google Dorking techniques step by step, I was able to refine the results and extract more useful and accurate information.

Each technique, like exact match, site filtering, and filetype search, plays an important role in improving the quality of results. Also, using multiple search engines helps in discovering additional data.

  

## 6. Practice Note  

For practice, the same techniques can be applied to:  

- crpf.gov.in  
- Any university website  
- Any public organization domain  

  
