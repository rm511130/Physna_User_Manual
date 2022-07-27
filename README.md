![Physna_Logo](./images/Physna_Logo.jpg)
# End User Guide v1.0.0
_(DRAFT)_
## Overview
This guide describes the features available to an End User of the Physna Enterprise Platform, a cloud-based 3D Geometric Search and Analysis solution enhanced by AI/ML. The intended audience includes anyone with access to a Physna Enterprise Graphics User Interface environment who needs to:

- upload models (CAD or SCAN files of parts or assemblies)
- organize models in folders and projects
- add or upload metadata associated to models
- search for models using 2D photos or 3D models
- search for models within other models 
- find matching models within a certain threshold of similarity
- find all duplicate models

_Note: depending on your Master Services Agreement and the features your company subscribed to, some of functionality described in this user guide may not be available to you_.

## Table of Contents

1. [What is Physna and what is it not?](#what-is-physna)
2. [How do I access a Physna environment?](#how-do-i-access)
3. [Navigating the Physna User Interface](#navigating-the-ui)
4. [Example use cases](#use-cases)
5. [Help and Support](#help_and_support)
6. [Architecture](#architecture)
7. Security _(...to be continued...)_
    - User Management
    - Okta Single Sign On
8. Certifications and Compliance _(...to be continued...)_
9. Service Levels and Known Limitations _(...to be continued...)_
10. FAQ (Frequently Asked Questions) _(...to be continued...)_
11. Terminology _(...to be continued...)_


## 1. What is Physna and what is it not?<a name="what-is-physna"></a>
- Physna is a company on a journey to empower human creativity by connecting the physical and digital worlds. Physna was founded on the principle that computers should be taught to accurately “think” in 3D – sorting and analyzing geometric objects like written code. Physna is building a future where people have the tools they need to design and analyze the parts and products that shape our world, to create and drive innovation in product design, 3D printing, augmented and virtual reality, gaming, healthcare, and beyond.
- Physna Enterprise is a cloud-based solution that employs patented 3D geometry based algorithms and AI/ML neural networks to search, match and compare 3D models.
- Physna is not a CAD, PDM or PLM tool. 
- Physna does, however, expose its functionality as consumable APIs that can be used to integrate Physna's functionality into existing IT Applications to enhance your company's business processes.
- Physna offers training, consulting and professional services through partner organizations for the customization of the Physna Base Connector that enables one-way or bi-directional movement of model and metadata information between PLM Solutions and Physna.

## 2. How do I access a Physna environment?<a name="how-do-i-access"></a>
- As a customer, your Sales and Customer Success teams will have given you a URL to access your firewalled, dedicated, and encrypted Physna Environment. The URL will probably follow the structure __https://my-company.physna.com__ where "__my-company__" is the name you agreed to use during initial implementation discussions with Physna's Customer Success team. 
- Ask your Business/Program/Project Leader or designated System Administrator what username you should use to log into your Physna environment. It will probably be your business Email Address or Single-Sign-On ID. If MFA (Multi-Factor Authentication) has been implemented, you will be asked to follow your company's standard MFA procedures.
- Use [Google's Chrome Browser](https://support.google.com/chrome/answer/95346) for better results. Other browsers have limitations that impede the use of all features.
- The Login Page is simple and comes with links in case you forget your username or password.

![Login-Page](./images/login_page_ext.jpg)

- When you first access a Physna Environment, you will be asked to set preferences or accept the storing of cookies on your device.

## 3. Navigating the Physna User Interface<a name="navigating-the-ui"><a/>
### 3a. Main Landing Page

- The main landing page, as seen below, is packed with features that are one click-away from delivering great insights into your 3D models. Please note that depending on your user role and the set of features your company has subscribed to use, some of the menu items may not be active or available to you.

![Unmarked_Main_Page](./images/Unmarked_Main_Page.jpg)

- Diving deeper into the main landing page features. Using the annotated diagram shown below, follow the sequence of numbers and their descriptions:

![Commented_Main_Page](./images/Commented_Main_Page_v1.jpg)

1. The search bar is for case-insensitive, partial or complete names of models, filenames, or metadata elements associated with the models. In the example above, the end user searched for "xx" and the results show all the models that contain "xx" in their names.
2. The triple horizontal lines open or close the sub-menu of advanced features and file management options that will be explained in a subsequent section of this user guide.  
3. The question mark icon opens a "Match Type" help screen that explains the 4 modalities of searches available to the end user directly from the main landing page.
    
    (i) Match: finds models that are geometrically similar to a chosen model
   
    (ii) Part Match: finds models into which your chosen model fits
   
    (iii) Scan Match: finds models when the chosen model is a high-poly scan by comparing bounding box volume parameters
   
    (iv) Classification Match: finds models using their geometric classification or predicted geometric classification
4. The radio buttons that switch the results between the 4 main modalities of searches available to the end user. The numbers between brackets indicate the number of hits, within the match tolerance (default value: 80%) specified immediately below. 
5. The match tolerance between 0 and 100% that is used to filter the search result set.
6. The model chosen as the subject for the searches. The model selection is controlled by clicking on the "Find Matches" URL next to any model displayed on the screen.
7. The result set with Match % details, model names and the ability to change the chosen model to be used in a "Find matches" query. In this section you can also click on "Add to Compare Cart" to add any given pair of models for comparison. Comparisons will be explained in a subsequent section of this user guide.  
8. Metadata fields associated horizontally to each other and to model in the same row. The titles of the columns can be dragged and moved, hidden and pinned to the left or the right of the displayed.

![ellipsis_v2](./images/ellipsis_v2.jpg)

9. Comparison Cart showing any two models to be compared. The models listed in the compare section can be cleared out from the cart or each model can be individually removed from the cart using the "x" next to it. Comparisons will be explained in a subsequent section of this user guide.
10. Download the contents of the page into using an Excel-friendly format.
11. Pagination control when the result sets can't be shown on a single page.
12. The three icons, in order from left to right, represent functionality that will be explained in a subsequent section of this user guide.
  
    (i) Upload models
  
    (ii) General settings
   
    (iii) User settings
    
13. The ability to toggle the display of results between the tighter table format shown above and the bigger thumbnails format shown below.

![bigger_thumbnails_results_page](./images/bigger_thumbnails_results_page.jpg)

### 3b. Uploading Files

For Physna to be able to index the geometry of your 3D models, you would need to first upload all necessary files to it. The upload button is in the upper-right corner of the page as shown here:

![upload-file-step-1-annotated](./images/upload-file-step-1-annotated.png) 

Pressing this button will open the upload page:

![upload-file-details-annotated](./images/upload-file-details-annotated.png)

1. Dropdown that lists all available folders in the environment and allows the user to select the target folder for the upload. The default is "Default Container"
2. Specify the units of measure (e.g., "inch", "mm")
3. When checked, it will prevent the upload of duplicate files
4. Pressing the "Upload Files" button will display standard file selection dialog. Choose one or more files from your local storage to be uploaded
5. List of recently uploaded files. Mostly for your information

Clicking the "Upload Files" button will open standard file selection dialog. The way that appears will depend on your operating system. Once you confirm your file selection the file will be uploaded to Physna and indexing will be initiated. Progress bar in the right side of the page will be displayed.

![upload-file-success](./images/upload-file-success.png)

At this time, the model should be visible in the destination folder. Physna will proceed through several stages of processing. When the processing state reaches "Finished", the model is ready for use. You can always see the status in the folder's page as shown previously.

## 4. Example Use Cases<a name="use-cases"><a/>

In the previous chapters we learned how to upload a file and how to navigate around the Physna's web site. In this chapter we will provide some examples of the types of practical operations one could perform.

### Searching for duplicate/similar parts

Provided that we have uploaded our inventory of parts to Physna as described earlier and all our models are in "Finished" state, we are ready to search for similar parts. 

With large teams and/or number of models, it is often possible to produce duplicate or at least very similar designs. This occurs even in cases where the company utilizes good PLM system and practice. In such cases, we find ourselves in a situation where the same part may be registered with different part numbers and has duplicate 3D models stored.

Physna can find if a model exists based on the geometry even in cases when the metadata differs. There are several types of searches, but the simplest one is the simple "Match".

First, we navigate to the folders where our model of interest is. This could be a model that we uploaded, and we would like to know if there is some other model that matches it with certain percent of confidence.

![duplicates-step-1](./images/duplicates-step-1.png)

For this example, we would like to see if "2.3 Shaft\_holder 1\_Trans Connector\_Front Axle\_Unreal Tractor\_by paX" has any models similar to it.

Selecting it from the list of models in the folder will show a context menu with links to "Find Matches" and "Add to Compare Cart". 

__NOTE: You do not need to scroll withing a folder to find your part. You can search for it by name if it is known. Enter the name in the search text field at the top of the main page to quickly navigate to the desired model.__

![duplicates-step-2](./images/duplicates-step-2.png)

To find similarities, click on "Find Matches".

![duplicates-step-3](./images/duplicates-step-3.png)

You can adjust the match percentage by moving the green slider bar left and right. In this example, with level of 70% we see two candidates. The first one shows match confidence of 86.88%, which indicates high level of similarity. Hovering over it will display the same options. This time, we would like to inspect visually the differences. To do that, we will click on "Add to Compare Cart" for that item.

![duplicates-step-4](./images/duplicates-step-4.png)

Notice that in the lower-left corner of the screen the "Compare Cart" now contains one item.

![duplicates-step-5](./images/duplicates-step-5.png)

Click "Add to Compare Cart" on the original part to also added it to the cart.

![duplicates-step-6](./images/duplicates-step-6.png)

With more than one items in the cart, we now see that the "Compare" button is enabled at the bottom of the panel.

![duplicates-step-7](./images/duplicates-step-7.png)

Click that button to open the Comparison Viewer.

![duplicates-step-8](./images/duplicates-step-8.png)

The default view is to show both models side by side, but you can also overlay them or use the "X-Ray" model. Those views offer different controls to adjust how they are presented for best effect. For example, you can adjust the opacity of the models.

![duplicates-step-9](./images/duplicates-step-9.png)

In many cases, it is sufficient to know the percentage of similarity. If it is 100%, you know that the two parts are exact duplicates even when they are registered with different names in your system. Comparing differences is most useful when you are trying to determine how and why the two are different.

_... to be continued ..._

## 5. Help and Support <a name="help_and_support"><a/>

You can find the details on how to contact the support team at Physna from the main hamburger menu on the main page. Click on the three horizontal lines icon to open the menu and select "Support" last item in the list. This will open a page explaining how to get in touch.

Alternatively, you can sent an e-mail to [info@physna.com](mailto:info@physna.com?subject=Physna%20Support) with subject "Support".

If you have a critical issue that requires immediate attention, please contact your Physna Account Team.

## 6. Architecture <a name="Architecture"><a/>    
    
Physna is a cloud-based platform installed as an isolated single tenant in order to guarantee complete control and isolation of your work and valuable data. The architecture diagram shown below represents all the key services used by Physna:
    
![architecture](./images/architecture.jpg)
    
    

