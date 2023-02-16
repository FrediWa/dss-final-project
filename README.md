# A Cascade (Hybrid) recommender system
## Created by me (Fredrik) and Samuel Granvik

This was the final project of the course "Decision support systems" where we were tasked to create a recommender system. Extra points were given for a hybrid system. Our approach is a cascade recommender system that mainly uses a collaborative model based recommender but then uses a simpler (more naive) content based for fallback for example for cold start.

Below is the original README with more notes and references. The notebooks also contain alot of details and reflections.

# dss-final-project

### Part 1 EDA
- Developed with Jupyter Anaconda
- Libraries used: pandas, numpy, matplotlib, pandas-profiling
- Encoding issues with geoplaces2.csv *Fixed
### Simple content based recommender
- Libraries used: pandas
- Label categorical data
- Check for similar rows using a simple distance metric
### Collaborative model based recommender
- Libraries used: pandas, numpy
- Create utility matrix and factorize using SVD
- Check for cosine similarity on hidden features V
- A Recommender class serves as an interface
### Hybrid recommender
- Inherit the Recommender class
- Implement a Cascade recommender
- Use the simple content based recommender if CFRS failed to make a recommendation 
## Resources
https://towardsdatascience.com/recommendation-system-matrix-factorization-d61978660b4b#:~:text=Matrix%20factorization%20is%20a%20collaborative,both%20item%20and%20user%20entities

https://towardsdatascience.com/how-does-collaborative-filtering-work-da56ea94e331

https://medium.com/analytics-vidhya/7-types-of-hybrid-recommendation-system-3e4f78266ad8

https://towardsdatascience.com/various-implementations-of-collaborative-filtering-100385c6dfe0

https://machinelearningmastery.com/using-singular-value-decomposition-to-build-a-recommender-system/
