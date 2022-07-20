![Physna_Logo](./images/Physna_Logo.jpg)
# End User Guide
## Overview
This guide describes the features available to an End User of the Physna Enterprise Platform, a SaaS based 3D Geometric Search and Analysis solution enhanced by AI/ML. The intended audience includes anyone with access to a Physna Enterprise Graphics User Interface environment who needs to:
- upload models (CAD or SCAN files of parts or assemblies)
- organize models in folders and projects
- add or upload metadata associated to models
- search for models using 2D photos or 3D models
- search for models within other models 
- find matching models within a certain threshold of similarity
- find all duplicate models

_Note: depending on your Master Services Agreement and the features your company subscribed to, some of functionality described in this user guide may not be available to you_.

## Table of Contents

1. What is Physna and what is it not?
2. How do I access a Physna environment?
3. Navigating the Physna User Interface
4. Solution SaaS, PaaS and API Architecture
5. Security
6. Certifications and Compliance
7. Help and Support
8. Service Levels and Known Limitations
9. FAQ (Frequently Asked Questions)
10. Terminology


## 1. What is Physna and what is it not?
- Physna is a company on a journey to empower human creativity by connecting the physical and digital worlds. Physna was founded on the principle that computers should be taught to accurately “think” in 3D – sorting and analyzing geometric objects like written code. Physna is building a future where people have the tools they need to design and analyze the parts and products that shape our world, to create and drive innovation in product design, 3D printing, augmented and virtual reality, gaming, healthcare, and beyond.
- Physna Enterprise is a SaaS based solution that employs patented 3D geometry based algorithms and AI/ML neural networks to search, match and compare 3D models.
- Physna is not a CAD, PDM or PLM tool. 
- Physna does, however, expose its functionality as consumable APIs that can be used to integrate Physna's functionality into existing IT Applications to enhance your companies business processes.
- Physna offers training, consulting and professional services through partner organizations for the customization of the Physna Base Connector that enables uni or bi-directional movement of model and metadata information between PLM Solutions and Physna.

## 2. How do I access a Physna environment?
- As a customer, your Sales and Customer Success teams will have given you a URL to access your firewalled, dedicated, and encrypted Physna Environment. The URL will probably follow the structure __https://my-company.physna.com__ where _my_company_ is the name you agreed to use during initial implementation discussions with Physna's Customer Success team. 
- Ask your Business/Program/Project Leader or designated System Administrator what username you should use to log into your Physna environment. It will probably be your business Email Address or Single-Sign-On ID. If MFA (Multi-Factor Authentication) has been implemented, you will be asked to follow your company's standard MFA procedures.
- Use [Google's Chrome Browser](https://support.google.com/chrome/answer/95346) for better results. Other browsers have limitations that impede the use of all features.
- The Login Page is simple and comes with links in case you forget your username or password.

![Login-Page](./images/login_page_ext.jpg)

- When you first access a Physna Environment, you will be asked to set preferences or accept the storing of cookies on your device.

## 3. Navigating the Physna User Interface
### 3a. Main Landing Page
- The main landing page, as seen below, is packed with features that are one click-away from deliverying great insights into your 3D models. Please note that depending on your user role and the set of features your company has subscribed to use, some of the menu items may not be active or available to you.
![Unmarked_Main_Page](./images/Unmarked_Main_Page.jpg)

- Diving deeper into the main landing page features. Using the annotaded diagram shown below, follow the sequence of numbers and their descriptions:
![Commented_Main_Page](./images/Commented_Main_Page_v1.jpg)

1. The search bar is for case-insensitive, partial or complete names of models, filenames, or metadata elements associated with the models. In the example above, the end user searched for "xx" and the results show all the models that contain "xx" in their names.
2. The tripple horizontal lines open up or close the sub-menu of advanced features and file management options that will be explained in a subsequent section of this user guide.  
3. The question mark icon opens up a "Match Type" help screen that explains the 4 modalities of searches available to the end user directly from the main landing page.
    
    (i) Ma.tch: finds models that are geometrically similar to a chosen model
   
    (ii) Part Match: finds models into which your chosen model fits
   
    (iii) Scan Match: finds models when the chosen model is a high-poly scan by comparing bounding box volume parameters
   
    (iv) Classification Match: finds models using their geometric classification or predicted geometric classification
4. The radio buttons that switch the results between the 4 main modalities of searches available to the end user. The numbers between brackets indicate the number of hits, within the match tolerance (default value: 80%) specified immediately below. 
5. The match tolerance between 0 and 100% that is used to filter the search result set.
6. The model chosen as the subject for the searches. The model selection is controlled by clicking on the "Find Matches" URL next to any model displayed on the screen.
7. The result set with Match % details, model names and the ability to change the chosen model to be used in a "Find mmatches" query. In this section you can also click on "Add to Compare Cart" to add any given pair of models for comparison. Comparisons will be explained in a subsequent section of this user guide.  
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
