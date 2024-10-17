## Medical-Notes-Categorization

I utilized text classification techniques to see how well notes that are taken by healthcare professionals can be understood and organized by machine learning algorithms.

## Context

The vast healthcare industry is an intricate and vital fabric of the livelihoods of billions across the world. Based on technological capabilities, different parts of the world vary in their tactics in making hospitals run more efficiently and treating patients more optimally. 

Extensive and time consuming paperwork is one of the largest areas of innovation happening in today's world. Doctors on average spend more time per day updating patient health records than actually spending time with their patients. This brief study showcases the importance and committment physicians have for maintaining clinical documentation: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4507919/. 

There are many avenues of patient note scribing that take place and I want to explore how technological systems can group notes, summarize a medical situation, and assess their meaning in the context of everyday healthcare dilemmas.

## Problem Statement

- We are trying to find innovative ways to classify pieces of textual data to a specific category through a classification model. This can eventually assist the healthcare system and its constituents in a variety of ways.
    - A hospital's virtual network of data will be better suited to carry out many tasks whether it is finding specific information, searching for potential patterns, or just general upkeep of patient history.
    -  All medical personnel whether it be doctors, nurses, and other necessary hospital staff will save large amounts of time avoiding paperwork and manual search and find missions for patient data.
    -  There will be more time for medical staff to spend with patients and to address necessary conditions and provide for treatments.

## Objective

Build a classification model to predict and sort patient notes to their correct medical specialty based on the text and context of the condition's description. 

## Data Dictionary

The Patient Notes dataset contains sample medical transcriptions for various medical specialties for about 5000 patient visits. It was scraped from [Transcribed Medical Transcription Sample Reports and Examples](https://www.mtsamples.com/) by [Tara Boyle](https://github.com/terrah27). The data gives us a brief overview of numerous, unique and everyday health conditions. 5 input variables were registered for each patient occurence.

* **Unnamed:** arbitrary record/row label
* **description:** short summary of transcription
* **medical_specialty:** category of transcription's medical classification 
* **sample_name:** title of transcription
* **transcription:** spoken and unspoken sample of medical report
* **keywords:** relevant keywords from transcription

## Findings & Solution

Our fine-tuned BERT model to classify diverse patient notes into different medical specialties should not be used. The accuracy of the model sits below the 30% ballpark and is way too low for real world application.

If executed at a preliminary level or once a higher accuracy is achieved, the following should be done.

  1. In order to ensure privacy and security of confidential patient data, a thorough check of both existing and new hospital data frameworks should be done. Accessability to the data as well as viewing and editing controls should be in compliance with federal, state, and local laws.   

  2. A well-thought-out timeline with metrics and guardrails should be presented to monitor the changes of such a model. It is imperative that hospitals and relative stakeholders start with a small sample of patients for their experimental trial of the model before exposing the entire patient notes database to the model. 

  3. This project will involve numerous departments and their employees across many stakeholders. A smooth transition into the current note gathering and storing process will be integral. Technology teams will also have to be onboarded and tasked with necessary roles for infrastructure upkeep along with their IT resources.
