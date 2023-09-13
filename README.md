# Bike Sharing Assignment
> A US bike-sharing provider __BoomBikes__ has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. > So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 

> In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

> They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to __understand the factors affecting the demand for these shared bikes in the American market__. The company wants to know:
>  - Which variables are significant in predicting the demand for shared bikes.
>  - How well those variables describe the bike demands

## Business Goal:
We are required to <mark>model the demand for shared bikes with the available independent variables.</mark> It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.


## Table of Contents

* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)


<!-- You can include any other section that is pertinent to your problem -->



## Conclusions
We have built a Linear Regression model to predict the demand of shared bikes in the American Market. The linear equation for the same is given by :__

<span style="color:'red">$ cnt = 0.2041 + 0.2556  \times  yr\_2019 - 0.1028  \times  holiday + 0.4736 \times temp - 0.1359 \times spring + 0.1060 \times winter - 0.0626 \times December - 0.0898 \times July - 0.0926 \times November - 0.3178 \times Light\_Snow-Rain - 0.0857 \times Mist\_Cloudy$</span>

Here,<br>
`cnt` is the demand of shared bikes on a particular day i.e. our target variable.

We can see in the above equation : 
1. __yr_2019__ is positively affecting demands i.e. Demands in 2019 has grown as compared to 2018.
2. __holiday__ is negatively impacting demands i.e. on holidays demands will be relatively less.
3. __temp__ is positively impacting demands i.e. increase in temperature, increases the demand.
4. __spring__ is negatively impacting demands i.e. during spring season demand is decreasing.
5. __winter__ is positively impacting demands i.e. during winter season demand is expected to be higher.
6. __December, July and November__ are negatively impacting demands i.e. during these months demand is lower.
7. __Light_Snow-Rain and Mist_Cloudy__ type weather is negatively impacting demands i.e. during snowy, rainy and misty weather demand is expected to decrease.

Out of all these features, <mark>__temp (temperature)__ is the most important factor affecting the demands of shared bikes in the American Market.</mark>

- We can see, that __Winter__ is positively affecting demands whereas the months of __November, December and January__ are negatively affecting the demands. This is due to the fact that USA has around 50 states and that's why __Winter__ can be during the months other December-January.
- __Temperature__ is positively affecting the demands because in USA , during winters it's mostly holiday and during summers it's not the case which is why demand is more.
- During __Light Snowy or Rainy__ weather cars are usually preferred as people would not like to go unprotected.
- During __holidays__, demand for shared bikes is low as people will stay at home during these days.

## :: Linear Regression Model's Peformance ::
__R_Squared:__`0.836`<br>
__Adj. R_Squared:__`0.832`<br>
__Model's R2_Score:__`0.813`
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- pandas - version 1.5.3
- numpy - version 1.23.5
- matplotlib - version 3.7.0
- matplotlib-inline - version 0.1.6
- seaborn - version 0.12.2

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Contact
Created by [@https://github.com/Anirudh1710/] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
