# Hotel Customer Segmentation

---
> ###*How can we group hotel customers to create targeted marketing strategies and tailored services?*

## Introduction
Customer segmentation is the marketing process of separating your customers into groups based on certain standard features and is a precursor to targeting and positioning. Customer segmentation becomes critical to address successful marketing strategies and create a compelling service portfolio. 

Historically, customer segmentation has been performed by sorting and classifying customers by standard features or behavior patterns. Clustering algorithms can unveil underlying trends and associations hidden from the classic analysis and help create a more effective customer segmentation.

## Methodology
The present project presents the customer/guest segmentation for a urban hotel in Lisbon, Portugal. We have used a dataset containing records of bookings of a city hotel [^1], with 31 variables describing 79,330 observations between the 1st of July of 2015 and the 31st of August 2017

The steps followed in this project are:
1. [Data wrangling](https://github.com/jvrnuno/Capstone-3/blob/main/notebooks/1_Collection_Inspection.ipynb)
	- Data collection
	- Feature extraction
	- Feature analysis and profiling
	- Quality assessment and data cleaning
2. [Exploratory data analysis (EDA)](https://github.com/jvrnuno/Capstone-3/blob/main/notebooks/2_exploratory_data_analysis.ipynb)
	- Feature transformation
	- Exploration of associations among categorical variables
	- Pairwise exploration of correlation in selected variables
4. [Preprocessing](https://github.com/jvrnuno/Capstone-3/blob/main/notebooks/3_Preprocessing.ipynb)
	- Sample selection
	- Categorical to cardinal transformation
	- Feature scaling
5. [Modeling and results](https://github.com/jvrnuno/Capstone-3/blob/main/notebooks/4_Modeling.ipynb)
	- Dimensionality reduction
	- Modeling with K-Means Clustering
		- K selection
		- Modeling and cluster sizes
	- Modeling with alternative algorithms
		- Agglomerative Hierarchical Clustering
		- DBSCAN Clustering
		- Mean-Shift Clustering
		- Expectation Maximization Clustering
	- Visualize results
	- Customer segments profiling

## Findings and conclusion
The present study shows an underlying segment structure in the data, and it is possible to establish five customer groups with similar characteristics. However, not all these groups have the same consistency and cohesion. Namely, samples from segments 0, 1, and 4 are closer, meaning that their attributes are more homogeneous. Segments 2 and 3 are more dispersed, and they can even be considered to not forming a group.

A customer profile based on the segments is presented below:

Customer Segment 0
: Tourist guest from a European country who arrives in August and stays two nights, usually makes a reservation two months in advance through an online agency. This customer is the least sensitive to prices, so he/she is willing to pay more for ancillary services.
Customer Segment 1
: Tourist national guest who comes in small groups and reserves a few rooms, usually stays two nights in October, and books three months in advance with an offline agency.
Customer Segment 2
: National business guest who arrives in February, stays one night. This client usually makes the reservation a week in advance, has a contract with the hotel, and pays a discount rate.
Customer Segment 3
: Tourist national guest who arrives in August and stays one night. He/She usually reserve three weeks in advance directly with the hotel, meaning that he/she has done previous research or is a returning customer. This client is not sensible to prices and is willing to pay a high rate.
Customer Segment 4
: National group guest who arrives in September and stays two nights, usually makes the reservation through a travel agency with 5-6 months in advance. This guest is very sensitive to prices and is very likely to cancel the reservation.

---
[^1] *Hotel booking demand datasets*. Nuno, Antonio; De Almeida, Ana; Nunes, Luis. Data In Brief n22 (2019), pag 41-49