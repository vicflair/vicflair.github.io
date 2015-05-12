# 120 interview questions

## Predictive modeling
1. (Given a dataset). Analyze this dataset and give me a model that can predict this response variable.
2. What could be some issues if the distribution of the test data is significantly different from the distribution of the training data?
3. What are some ways I can make my model more robust to outliers?
4. What are some differences you would expect in a model that minimizes squared error, versus a model that minimizes absolute error? In which cases would each error metric be appropriate?
5. What error metric would...
6. What are various ways...
7. What is regularization and where might it be helpful? What is an example of using regularization in a model?
8. Why might it be preferable to include fewer predictors over many?
9. Given training data on tweets and their retwees, how would you predict the number of retweets of a given tweet after 7 days after only observing 2 days worth of data?
10. How could you collect and analyze data to use social media to predict the weather?
11. How would you construct a feed to show relevant content for a site that involves user interactions with items?
12. How would you design the people you may know feature on LinkedIn or Facebook?
13. How would you predict who someone may want to send a Snapchat or Gmail to?
14. How would you suggest to a franchise where to open a new store?
15. In search engine, given partial data on what the user has typed, how would you predict the user's eventual search query?
16. Given a database of all...
17. You're Uber and you want...
18. How would you build a model to predict a March Madness bracket?
19. You want to run a regression to predict the probability of a flight delay, but there are flights with delays of up to 12 hours that are really messing up your model. How can you address this?

## Programming
1. Write a function to calculate all possible assignment vectors of *2n* users, where *n* users are assigned to group 0 (control), and *n* users are assigned to group 1 (treatment).
2. Given a list of tweets, determine the top 10 most used hashtags.
3. Program an algorithm to find the best approximate solution to the knapsack problem in a given time.
4. Program an algorithm to find the best approximate solution to the travelling salesman problem in a given time.
5. You have a stream of data coming in of size *n*, but you don't know what n is ahead of time...
6. Write an algorithm that...
7. Given a list of numbers,...
8. When can parallelism make your algorithms run faster? When could it make your algorithms run slower?
9. What are the different types of joins? What are the differences between them?
10. Why might a join on a subquery be slow? How might you speed it up?
11. Describe the difference between primary keys and foreign keys in a SQL database.
12. Given a *COURSES* table with columns *course_id* and *course_name*, a *FACULTY* table with columns *faculty_id* and *faculty_name*, and a *COURSE_FACULTY* table with columns *faculty_id* and *course_id*, how would you return a list of faculty who teach a course given the name of a course.
13. Given a *IMPRESSIONS* table with *ad_id*, *click* (an indicator that the ad was clicked), and *date*, write a SQL query that will tell me the click-through-rate of each ad by month.
14. Write a query that returns the name of each department and a count of the number of employees in each: ...

## Probability
1. Bobo the amoeba has a 25%, 25%, and 50% chance of producing 0, 1, or 2 offspring, respectively. Each of Bobo's descendants also have the same probabilities. What is the probability that Bobo's lineage dies out?
2. In any 15-minute interval, there is a 20% probability that you will see at least one shooting star. What is the probability that you see at least one shooting star in the period of an hour?
3. How can you generate a (uniform) random number between 1-7 with only a standard die?
4. How can you get a fair coin toss if somone hands you a coin that is weighted to...
5. You have a 50-50 mix...
6. Given draws from a normal distribution with known parameters, how can you simulate draws from a uniform distribution?
7. A certain couple tells you that they have two children, at least one of which is a girl. (Given this information) What is the probability that they 
have two girls?
8. You have a group of couples that decide to have children until they have their first girl, after which they stop having children. WHat is the expected gender ratio of the children that are born? What is the expected number of children each couple will have?
9. How many ways can you split 12 people into 3 teams of 4?
10. Your hash function assigns each object to a number between 1:10, each with equal probability. With 10 objects, what is the probability of a hash collision? What is the expected number of hash collisions? What is the expected number of hashes that are unusued?
11. You call 2 UberX's and 3 Lyfts. If the time each takes to reach you is IID, what is the probability that all the Lyfts arrive first? What is the probability that all the UberX's arrive first?
12. I write a program that should print out all the numbers from 1 to 300, but prints out Fizz instead if the number is divisible by 3, Buzz instead if the number is divisible by 5, and FizzBuzz if the number...
13. On a dating site, users...
14. A lazy high school senior types up application and envelopes to *n* different colleges, but puts the applications randomly into the envelopes. What is the expected number of applications that went to the right college?
15. Let's say you have a very tall father. On average, what would you expect the height of his son to be? Taller, equal, or shorter? What if you had a very short father?
16. What's the expected number of coin flips until you get two heads in a row? What's the expected number of coin flips until you get two tails in a row?
17. Let's say we play a game where I keep flipping a coin until I get heads. If the first time I get heads is on the *n*th coin, then I pay you *2n-1* dollars. How much would you pay me to play this game.
18. You have two coins, one of which is fair and comes up heads with a probability 1/2, and the other which is biased and comes up heads with probability 3/4. You randomly pick a coin and flip it twice, and get heads both times. What is the probability that you picked the fair coin.
19. You have a 0.1% chance of picking up a coin with both heads, and a 99.9% chance that you pick up a fair coin. You flip your coin and it comes up heads 10 times. What's the chance that you pick up the fair coin, ...

- Simpson's paradox. Example from wikipedia, explain?
- Poor use of averages. You have two new features *A* and *B* on the front page. In testing, you found that over *A*'s average conversion rate in Q1 was higher than *B*'s in Q1, and likewise for Q2. But, *B*'s average conversion rate over both quarters, i.e. the 1st half of the year, is *higher* than *A*'s. What could be the explanation? (like the college acceptance scandal, or batting averages, there are different number of samples for each measure: *A* vs *B* and Q1 vs Q2)

## Statistical inference
1. In an A/B test, how can you check if assignment to the various buckets was truly random?
2. What might be the benefits of running an A/A, where you have two buckets who are exposed the exact same product?
3. What would be the hazards of letting users sneak a peek at the other bucket in an A/B test?
4. What would be some issues if blogs decide to cover one of your experimental groups?
5. How would you conduct an A/B test on an opt-in feature?
6. How would you run an...?
7. How would you run an ... extremely right-skewed?
8. I have two different...
9. What is a p-value? What is the difference between type-1 and type-2 error?
10. You are AirBnB and you want to test the hypothesis that a greater number of photographs increases the chances that a buyer selects the listing. How would you test this hypothesis?
11. How would you design an experiment to determine the impact of latency on user engagement?
12. What is maximum likelihood estimation? Could there be any case where it doesn't exist?
13. What's the difference between a MAP, MOM, MLE estimator? In which cases would you want to use each?
14. What is a confidence interval and how do you interpret it?
15. What is unbiased as a property of an estimator? Is this always a desirable property when performing inference? What about in data analysis or predictive modeling?

## Data analysis
1. (Given a dataset) Analyze this dataset and tell me what you can learn from it.
2. What is *R^2*? What are some other metrics that could be better than *R^2* and why?
3. What is the curse of dimensionality?
4. Is more data always better?
5. What are advantages of plotting your data before performing analysis?
6. How can you make sure you don't analyze something that ends up meaningless...?
7. What is the role of trial...
8. How can you determine ...
9. How do you deal with some of your predictors being missing?
10. You have several variables that are positively correlated with your response, and you think combining all of the variables could give you a good prediction of your response. However, you see that in the multiple linear regression, one of the weathers on the predictors is negative. What could be the issue?
11. Let's say you're given an unfeasible amount of predictors in a predictive modeling task. What are some ways to make the prediction more feasible?
12. Now you have a feasible amount of predictors, but you're fairly sure you don't need all of them. How would you perform feature selection on the dataset?
13. Your linear regression didn't run and communicates that there are an infinite number of best estimates for the regression coefficients. What could be wrong?
14. You run your regression on different subsets of your data, and find that in each subset, the beta value for a certain variable varies wildly.
15. What is the main idea behind ensemble learning? If I had many different models that predicted the same response variable, what might I want to do to incorporate all of the models? Would you expect this to perform better than an individual model or worse?
16. Given that you have...
17. How could you use GPS...
18. Given accelerometer...
19. Given position data of NBA players in a season's games, how would you evaluate a basketball player's defensive ability?
20. How would you quantify the influence of a Twitter user?
21. Given location data of golf balls in games, how would you construct a model that can advise golfers where to aim?
22. Given location data of golf balls in games, how would you construct a model that can advise golfers where to aim?
23. You have 100 mathletes and 100 math problems. Each mathlete gets to choose 10 problems to solve. Given data on who got what problem correct, how would you rank the problems in terms of difficulty?
24. You have 5000 people that rank 10 sushis in terms of saltiness. How would you aggregate this data to estimate the true saltiness rank in each sushi?
25. Given data on congressional bills and which congressional representatives co-sponsored the bills, how would you determine which other representatives are most similar to yours in voting behavior? How would you evaluate who is the most liberal? Most republican? Most bipartisan?
26. How would you come up with an algorithm to detect plagiarism in online content?
27. You have data on all purchases of customers at a grocery store. Describe to me...
28. Let's say you're building...

## Product metrics
1. What would be good metrics of success for an advertising-driven consumer product? (Buzzfeed, YouTube, Google Search, etc.) A service-driven consumer product? (Uber, Flickr, Venmo, etc.)
2. What would be good metrics of success for a productivity tool? (Evernote, Asana, Google Doc,s etc.) A MOOC? (edX, Coursera, Udacity, etc.)
3. What would be good metrics of success for an e-commerce product? (Etsy, Groupon, Birchbox, etc.) A subscription product? (Netflix, Birchbox, Hulu, etc.) Premium subscriptions? (OKCupid, LinkedIn, Spotify, etc.)
4. What would be good... product that relies...
5. What would be good.... that offered in-app...
6. A certain metric is violating your expectations by going down or up more than you expect. How would you try to identify the cause of the change?
7. Growth for total number of tweets sent has been slow this month. What data would you look at to determine the cause of the problem?
8. You're a restaurant and are approached by Groupon to run a deal. What data would you ask from them in order to determine whether or not to do the deal?
9. You are tasked with improving the efficiency of a subway system. Where would you start?
10. Say you are working on Facebook News Feed. What would be some metrics that you think are important? How would you make the news each person gets more relevant?
11. How would you measure the impact that sponsored stories on Facebook News Feed have on user engagement? How would you determine the optimum balance between sponsored stories and organic content on a user's News Feed?
12. You are on the data science team at Uber and you are asked to start thining about surge pricing. What would be the objectives of such a product and how would you start looking into this?
13. Say that you are Netflix. How would you determine what original series you should invest in and create?
14. What kind of services would find churn...
15. Let's say that you're...

## Communication
1. Explain to me a technical concept related to the role that you're interviewing for.
2. Introduce me to something you're passionate about.
3. How would you explain an A/B test to an engineer with no statistics background? A linear regression?
4. How would you explain a confidence interval to an engineer with no statistics background? What does 95% confidence mean?
5. How would you explain to a group of senior executives why data is important?
6. Tell me about a data project...
7. Tell me about a dataset...
8. What's your favorite algorithm....
9. How could you help generate public understanding towards the importance of using data to generate insights?
10. How would you convince a government agency to relase their data in a publicly accessible API?
11. I'm a local business owner operating a small restaurant. Convince me to switch my advertising budget from print to internet.
