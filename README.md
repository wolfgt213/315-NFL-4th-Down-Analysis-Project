# 315-NFL-4th-Down-Analysis-Project

## 1. Team Information
**Team Name: NFL Data Analysts** 

**Contributors:**
- Grant Wolf
- CJ Persico
- Logan Eldredge

## 2. Objective and Motivation
### Objective


### Motivation

## 3. Dataset Description

**Dataset Name:** NFLverse

**Source:** [https://nflverse.nflverse.com/](https://github.com/nflverse/nflverse/)

**Data Format:** CVS File

**Description:** Large set of packages of data from the National Football League that include play-by-play data back to 1999, season simulations, 4th down analysis, 

**Data Preparation:**

## 4. Research Questions and Expected Answers

### Question 1: 
- **Question:** How does the number of yards needed for a fourth down conversion affect the probability of having a successful fourth down conversion?
- **Expected Answer:** We will plot distance needed for conversion on the x-axis (units of yards) against successful fourth down conversion probability on the y-axis (as a percentage). We will use data fitting to analyze this relationship. We generally expect the conversion success rate to increase as yards needed to convert decreases. We will calculate 95% confidence intervals for successful fourth down conversions at different distances to convert. Maybe 5: ("4th and Inches" (<1 yard), "4th and Short" (1-<3 yards), "4th and Medium" (3-<7 yards), "4th and Long" (7-<15 yards), and "4th and Forever" (>15 yards).
- **Potential Benefit:** This can help us determine that if you are closer to the yard to gain, that your chances of obtaining a new set of downs increases.

### Question 2: 
- **Question:** How does field position affect the probability of having a successful fourth down conversion?
- **Expected Answer:** We will plot distance to the goal line on the x-axis (units of yards) against successful fourth down conversion probability on the y-axis (as a percentage). We will use data fitting to analyze this relationship. We hypothesize that the conversion success rate increases as distance to the goal line increases because the defense has more open field to defend. We will calculate 95% confidence intervals for successful fourth down conversions at different distance to the goal line. Maybe 10: (0-1 yards, 1-4 yards, 4-9 yards, 9-16 yards, 16-25 yards, 25-36 yards, 36-49 yards, 49-64 yards, 64-81 yards, 81-100 yards)
- **Potential Benefit:** This will help us determine if the position on the field truly influences the probability of a 4th down conversion due to the remainder of the field to go.

### Question 3: 
- **Question:** How does home field advantage affect the probability of having a successful fourth down conversion?
- **Expected Answer:** We will make a bar graph with two bars on the x-axis. One bar will represent home teams, while the other bar will represent away teams. The y-axis will be successful fourth down conversion rate (as a percentage). We expect the successful fourth down conversion rate to be greater for the teams with the home field advantage. Additionally, we will use a chi-squared test to determine if the home field advantage for fourth down conversion rate is statistically significant.
- **Potential Benefit:** This will help us determine if you're the home or away team influences the probability of a 4th down conversion.

## 5. Introduction and Context


## 6. Implementation Details: Methods, Metrics, Tools, and Plots

### Question 1: How does the number of yards needed for a fourth down conversion affect the probability of having a successful fourth down conversion?
**Method:**
We will use the NFLverse 2025-2026 season play-by-play dataset to analyze the applicable columns including yards needed to convert (ydstogo), successful fourth down conversions (fourth_down_converted), and failed fourth down conversions (fourth_down_failed). Then, we will calculate 95% confidence intervals at the various ranges stated above. After inputting the data, we can use equations to find the appropriate data fitting method.

**Metrics:**
- Number of fourth down attempts for each chosen distance interval
- Number of successful fourth down attempts for each chosen distance interval
- Percentage of conversion success rate for each chosen distance interval
- 95% confidence interval for each conversion success rate

**Python Tools and Packages:**
- Pandas for data analysis
- NumPy for calculations
- SciPy for statistics
- Matplotlib for plotting

**Visualization:**
We will plot this data on a graph. The x-axis will be yards needed for conversion (yards). The y-axis will be conversion success rate (%). Error bars will indicate the 95% intervals of our chosen distance intervals. It will include an appropriate trendline.

**Interpretation:**
We expect conversion success rates to decrease as yard needed to convert increase. The confidence intervals will determine the precision of our findings. The trendline will show us the overall relationship.

### Question 2: How does field position affect the probability of having a successful fourth down conversion?
**Method:**
We will use the NFLverse 2025-2026 season play-by-play dataset to analyze the applicable columns including distance from the goal line (yardline_100), successful fourth down conversions (fourth_down_converted), and failed fourth down conversions (fourth_down_failed). Then we will calculate 95% confidence intervals at the various locations along the field. After inputting the data, we can use equations to find the appropriate data fitting method.

**Metrics:**
- Number of fourth downs attempted for each distance interval along the length of the field
- Number of successful fourth down attempts for each chosen distance interval
- Percentage of conversion success rate for each chosen distance interval
- 95% confidence interval for each conversion success rate

**Python Tools and Packages:**
- Pandas for data analysis
- NumPy for calculations
- SciPy for statistics
- Matplotlib for plotting

**Visualization:**
We will plot this data on a graph. The x-axis will be yards from the goal line. The y-axis will be conversion success rate (%). Error bars will indicate the 95% intervals of our chosen distance intervals. It will include an appropriate trendline.

**Interpretation:**
We expect that the further from the goal line, the higher the chance of a conversion due to the expanded area that the defense needs to cover, while the closer to the goal line, the harder it is to accomplish a conversion.

### Question 3: How does home field advantage affect the probability of having a successful fourth down conversion?
**Method:**
We will use the NFLverse 2025-2026 season play-by-play dataset to analyze the application columns including Possession (posteam), who the home team was (home_team), successful fourth down conversions (fourth_down_converted), and failed fourth down conversions (fourth_down_failed). We will then perform a Chi squared test to determine if the home field advantage for fourth down conversion rate is statistically significant,

**Metrics:**
- Who has possession of the ball
- Who the home team is
- Number of successful 4th down conversions
- Chi squared test to see if statistically significant 

**Python Tools and Packages:**
- Pandas for data analysis
- NumPy for calculations
- SciPy for statistics
- Matplotlib for plotting

**Visualization:**
A bar graph with two bars along the x-axis. One will represent the home teams, while the other represents the away teams. The y-axis will be successful fourth down conversion rate (as a percentage).

**Interpretation:**
We expect that the successful fourth down conversion rate will be greater for the home team rather than the away team.

## 7. Project Structure
- `README.md` — Project description and documentation
- `data/` — Dataset or instructions for obtaining it
- `src/` — Python source code
- `figures/` — Generated plots and visualizations
- `report/` — Final report materials

## 8. Results: Answers to the Questions
[Placeholder for results, charts, analysis, and answers to the research
questions. To be completed in a later phase.]

## 9. Conclusions
[Placeholder for conclusions, key findings, limitations, and future work.]

## 10. Actions That Need to Be Completed
- [ ] Finalize the dataset and verify its quality.
- [ ] Complete data cleaning and preparation.
- [ ] Implement the analysis methods.
- [ ] Calculate the selected metrics.
- [ ] Generate and interpret visualizations.
- [ ] Answer each research question.
- [ ] Complete the final presentation and live demonstration.
- [ ] Complete the final report and source code.

**Current Issues and Challenges:**
[Describe outstanding problems, dependencies, or challenges for each
incomplete task.]

## 11. References and Source Files
- Dataset source and URL: NFLverse [https://nflverse.nflverse.com/](https://github.com/nflverse/nflverse-data/releases/download/pbp/play_by_play_2025.csv) 
- [Research papers, articles, or documentation]
- [Python library documentation]
- [Other relevant sources]



