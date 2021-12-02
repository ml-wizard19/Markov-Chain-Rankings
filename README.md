# Markov Chain Rankings
This repository contains the code used to scrape NBA results from basketball-reference and also test the accuracy of the markov method for sports rankings. Rankings for the NBA playoffs for all seasons dating back to the NBA/ABA merger were created using markov chains and the accuracy was tested against that of the NBA official seeding. The paper associated with the code is also included in the repository.

### Workflow
* Scrape regular season results, playoff results, and regular season standings from basketball reference (1977 - 2017)
* Form a voting matrix using a specified alpha level using regular season results for each year
* Get the team ratings for each season (and subsequent rankings) by solving the matrix for its stationary distribution (Markov Method)
* Use both the Markov Rankings and regular season standings to make predictions for the playoff series for each season
* Compare the total accuracies of the different ranking methods