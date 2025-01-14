# A simple Oasis Ransomware Model
A ransomware attritional portfolio model for use with the Oasis Loss Modelling Framework. This model uses a portfolio as an input to generate monte carlo ransomware losses which take account of the company's revenue, sectors, and country. The model does not take into account the security posture of each individual company, it simply assumes a basis risk for for different revenue, sector, and country combinations. However, it does take account that some ransomware threat actors are more prolific than others, and make different targetting choices. 

The losses will be modelled in USD, and the revenue of the companies should be provided in USD. However, the location of the company's HQ can be given different country codes. Thus the model is global in capability, and is senstive to sector and company revenue as well. The model is primarily designed for insurance or reinsurance companies to use, but may be useful for policy makers at the government or international levels as well. 

The model has many assumptions, and is built with the expectation that it will need yearly updates as ransomware evolves. An increase in threat actors or decrease in ransom paid percentages or change in the number of companies above a certain revenue threshold are all example reasons these updates are necessary. However, we do believe that estimating the cost to society of ransomware events leads to better spending on defences or capacity building, and it is worth considering the cost of ransomware events with economic modelling accordingly.

# Model assumptions:

All models must have assumptions, and we try to openly declare ours here. We believe the creation of a model is like a thesis, it should be clearly stated before it can be defended. Here we clearly state the assumptions we had and the effect they have on the model, so that others may choose to change them, or use them as designed.

## Ransomware losses can be caused by privacy and data breach, or digital asset and recovery

Modern ransomware switches between multiple tactics, and thus we needed different sub coverages with in the model for incident response, digital asset and recovery, and extortion. We plan for business interruption in a future update of the model, and will consider other sub-coverages when new research comes to light that expllains them adequently.

## Ransom paid ratio:

Ransomware has different cost profiles if you pay or don't pay the ransom. We had to assume some level of payment across the events generated in the portofio, and so we chose 30% of incidents involve a ransom being paid, and 70% involve only loss costs and no ransom payment. This number of course might be different because of an insurers approach to the problem, but we chose what we believe to be an industry average. If you need the model tuned to a different ratio of payment, get in touch.

## Country GDP is a strong predictor of frequency:

Countries with higher GDP suffer more ransomware events than those that do not. So the country of the companies in the portfolio will change the frequency with which they are sampled for losses.

## Revenue drives both frequency and severity effects:

Larger companies are hit more frequently than smaller companies, but the relative damage to smaller companies can be greater. We have baked this into our construction of the model.

## Different threat actors drive different effects in frequency and severity:

We have created sectoral, country, and revenue, variation for each of the threat actors in the model. So in the future, the emergent effects of their interactions can be studied. Thus if new threat actors arrive on the scene, we can plug them easily into future versions, and retire groups who are no longer active.
