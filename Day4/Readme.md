# Day 5 – Image & Geolocation Intelligence (IMINT + GEOINT)
## Image Analysis, Metadata & Geolocation Verification  


## 1. Objective  

In this task, I performed Image Intelligence (IMINT) and Geolocation Intelligence (GEOINT) to analyze a digital image. The goal was to extract hidden metadata, verify location and time, detect manipulation, and identify the origin of the image using open-source tools.



## 2. Target  

- **Primary Target:** image.jpg  
- **Type:** Digital Image Evidence  



## 3. Tools Used  

- Exif.tools (browser-based)    
- Google Lens  
- TinEye  
- FotoForensics  
- OpenStreetMap 



## 4. Workflow  



## Step 1: Metadata Extraction (Image → Hidden Data)  

**Input I used:**  
![image.jpg](Images/image.jpg)

**Tool I used:**  
[exif.tools](https://exif.tools/exiftool)

**What I did:**  
I uploaded the image and extracted metadata.

**Screenshot:**  
![Step 1](Images/Step.png)

**What I observed:**  
- DateTimeOriginal (photo capture time)  
- GPS Latitude & Longitude  
- Camera Make and Model  
- Software used (Photoshop, etc.)  
- Embedded thumbnail  

**What I understood:**  
Metadata reveals hidden information about how, when, and where the image was captured. Absence of metadata may indicate removal or privacy settings.



## Step 2: GPS Coordinate Mapping (Image → Location)  

**Input I used:**  
Extracted latitude and longitude  

**Tool I used:**  
Google Maps / Google Earth  

**What I did:**  
I entered the GPS coordinates into Google Maps.

**Screenshot:**  
![Step 2](Images/Step2.png)

**What I observed:**  
- Exact location of capture  
- Terrain and surroundings  
- Match or mismatch with claimed location  

**What I understood:**  
GPS data helps confirm whether the image was taken at the claimed location. Missing GPS data itself is an important finding.



## Step 3: Date and Time Verification  

**What I did:**  
I compared metadata time with the claimed timeline.

**Screenshot:**  
![Step 3](Images/Step3_Time_Verification.png)

**What I observed:**  
- Metadata date vs claimed date  
- Possible mismatch due to incorrect device clock  

**What I understood:**  
Camera timestamps are not always reliable and must be validated with other evidence.



## Step 4: Reverse Image Search (Origin Detection – First Pass)  

**Tool I used:**  
Google Images / Google Lens  

**What I did:**  
I uploaded the image to search engines.

**Screenshot:**  
![Step 4](Images/Step4.png)

**What I observed:**  
- Same image on other websites  
- News articles or blog posts  
- Earlier appearances  

**What I understood:**  
If the image appears before the claimed event date, it is likely reused or misleading.



## Step 5: Reverse Image Search (Deep Search)  

**Tool I used:**  
TinEye  

**What I did:**  
I performed deeper reverse searches.

**Screenshots:**  
![TinEye](Images/Step5.png)  

**What I observed:**  
- TinEye shows oldest indexed appearance  

**What I understood:**  
Using multiple engines improves accuracy and ensures wider coverage.



## Step 6: Image Manipulation Detection  

**Tool I used:**  
FotoForensics 

**What I did:**  
I performed Error Level Analysis (ELA).

**Screenshot:**  
![Step 6](Images/Step6.png)

**What I observed:**  
- Uniform patterns → likely original  
- Bright or inconsistent patches → possible editing  
- Copy-paste artifacts  

**What I understood:**  
ELA helps detect tampering or manipulation.



## Step 7: Visual Geolocation (Without GPS Data)  

**What I did:**  
I manually analyzed the image.

**Screenshot:**  
![Step 7](Images/Step7.png)

**What I observed:**  
- Terrain (forest, hills, plains)  
- Vegetation type  
- Road structure  
- Language on signboards  
- Building styles  
- Skyline or mountains  

**What I understood:**  
Visual clues help estimate location when metadata is missing.



## Step 8: Geolocation Verification (Maps & Terrain Matching)  

**Tool I used:**  
Google Earth / Google Maps / OpenStreetMap  

**What I did:**  
I cross-checked the suspected location.

**Screenshot:**  
![Step 8](Images/Step8.png)

**What I observed:**  
- Terrain matching  
- Road alignment  
- Landmark similarity  

**What I understood:**  
Matching terrain and structures confirms or rejects the suspected location.

## 5. Conclusion  

From this task, I understood that image intelligence involves multiple verification layers. By combining metadata analysis, reverse image search, geolocation, and forensic techniques, it is possible to validate the authenticity, origin, and timeline of an image.



## 6. Practice Note  

For practice, the same techniques can be applied to:  

- Social media images  
- News reports  
- Viral misinformation images  
- Satellite imagery  
