# Customer Segmentation - Four Steps to ensure Efficient Physician Targeting and Segmentation
This is to demonstrate and automate the use of python to effectively target and segment customers based on their sales potential, academia/speaker influence and behavioral attributes

I wrote this article on https://iotmusings.com/targeting-segmentation/
(Will expand and demonstrate how it was done)

Text from the article is pasted below
---------------------------------------------
According to a study in 2012 –  ‘Six minutes’ – that was the average length of a medical sales representative’s call with a healthcare provider (HCP). It has probably reduced by half at the time of writing this article. The cost of training, hiring specialized sales force could be upwards of $300,000.

Because sales force time is an expensive and limited resource, efforts are concentrated on high potential customers. The physicians of interest are assigned ranks which signify potential for prescription sales volume.

Sales promotion efforts are increasingly concentrated on a small group of highly prescribing physicians
You don’t have to look far to stumble upon an alternative for 80:20 rule in pharmaceutical sales targeting. There are instances where 30% of prescribing physicians generate more than 80% of of prescriptions.

Highly effective targeting and a pointed marketing strategy is therefore, one of the most imperative activities to gain market share.

Eligible Doctor Universe:
The analytic exercise generally begins with an eligible doctor universe. Specifically all the eligible doctors who could prescribe for the therapeutic area of interest.

An example of eligible physician universe for an Oncology drug: There are about 16,000 physicians in United States that have Oncology Specialties:

This is of course a starting point. This physician universe will be sliced before a final target list is arrived at.



General Rules Applied: Note that depending on the Therapeutic area, you could subset using more filters.
For example:
Start with 16,000 Physicians with Oncology Specialty
Apply filter on Market Basket (only if you know your competitors) and have competitive data to support it. For the purpose of this article, I am assuming that through efforts of markets research and secondary data analytics, competition has been determined (based on mechanism of action of the drug, alternative therapies, molecule properties etc.)
Apply Indication/Diagnosis Rule: Only physicians who have prescribed at least one prescription for specific ICD9/ICD10
Filter by Approved Specialties: If its a Lung Cancer Drug, you may not want to include Gynecologic Specialty physicians
Arrive at a Final Target Universe
Stratification or Segmenting your Final Target Universe –> Final Target List
The target universe is segmented into deciles based on Prescription Volume. You could use past 12 months of historical prescription volume (or Claims Data).



Companies select the top deciles for direct sales promotion and create a target list on whom sales representatives will call on to promote a therapeutic portfolio or particular product.



Case for Behavioral Segmentation
It is in the best interest to do more than just the traditional segmentation based on sales volume. Behavioral aspects such as: 

Is the prescribing physician a KOL?
Is the Physician a Trialist?
Has the physician been in a capacity of a speaker?
Social Media Posts (Assign a score based on scraped data/tweets etc.)
‘Is the Prescriber an Early Adopter, Middle of the Road or a Late Adopter can be crucial especially if you are looking to launch a new Indication/Product?



How to incorporate the behavioral aspect of a Prescriber?
Update the previous decile to incorporate behavioral aspects. An internal discussion should get you aligned on how much (or less) important these aspects here.

A combination of: IF PREV_DECILE = 7 AND KOL_FLAG=1 THEN NEW_DECILE=8  should help you incorporate these metrics.



Plan of Action post Targeting & Segmentation Exercise: Develop a Call Plan
The Final Target List that is obtained after segmentation exercise paves a way to develop a plan of action:

For instance: Decile 6 – Decile 9 may be detailed more than 6 times in a quarter (Call Plan) and Decile 2 – Decile 5 may be detailed once a month

There are a  lot of Use-Cases for Advanced Analytics in Physician Targeting as quantitative and behavioral aspects will merge for highly specialized targeting.
