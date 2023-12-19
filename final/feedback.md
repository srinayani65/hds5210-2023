# Feedback on your final

**Final Score: 57/60**

The grading rubric for the final can be found in GitHub: https://github.com/paulboal/hds5210-2023/blob/main/final/final-instructions.pdf

**Functional Requirements**
* 5 points - Uses data from at least two different sources: local file, internet, web service, relational database, AWS S3, etc; and formats: CSV, JSON, database, XML, Excel, etc
* 5 points - Data from multiple sources has to be joined together at least twice
* 5 points - Data is aggregated or pivoted at least twice during the program
* 5 points - Some kind of field-level transformation is performed at least 5 times
* 5 points - The program creates 3 or more data visualizations 
* 5 points - The program serves a theoretical purpose described in documentation, that could potentially do something in healthcare or another industry of interest

**Modularity / Style**
* 15 points - The code is broken up into various functions or classes to make testing and reuse easier

**Documentation and Professionalism**
* 15 points - All functions are documented and notebook cells include annotations and explanations.


**(-2) Your "prepare_data" function has a lot going on and it would have been helpful to provide a few more comments about what was happening there.  A few notes on this function:**
* It's bad practice to iterated through dataframes.  You can almost always do a vectorized operation instead.
* You did a lot of mapping from one description/column domain to another. There's a dataframe function called `.map(dict)` that makes this much easier. You could have eliminated more than 50% of the code in this function.
* It's confusing that you split the data into Male/Female and then just reconcatenated it.

**(-1) Your "get_status_count" was god to have encapsulated in a function, but it probably would have been better to do this kind of operation with a pivot table and filters.**

**Overall, a solid final project.  Nice work!**