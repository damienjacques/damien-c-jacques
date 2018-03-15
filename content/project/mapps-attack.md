+++
# Date this page was created.
date = "2016-04-27"

# Project title.
title = "Mapps Attack"

# Project summary to display on homepage.
summary = "Project presented at the International Space Apps Challenge solving the *Where on Earth* challenge."

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "MappsAttack.jpg"

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["space-apps", "fun", "game", "land-cover", "crowdsourcing"]

# Optional external URL for project (replaces project detail page).
external_link = "" #https://2014.spaceappschallenge.org/project/mapps-attack/

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).   insert img ![World Map of Köppen−Geiger Climate Classification.](/img/stratification.jpg)

[header]
image = "headers/MappsAttack.jpg"
caption = "Project presented at the International Space Apps Challenge"

+++
Got the heart of an explorer ? Be involved in a thrilling race to conquer the world. Over deserts, seas and mountains, be the first pioneer to tread on unchartered territory. Always be on your guard, you are not alone in this undertaking and the enemy might be nearby. Protect your land against invaders and consolidate your positions. The earth is limited and therefore, a highly coveted resource. Hurry, and take the lion’s share !

Through a highly convenient and addictive game application, the project aims to develop a database of land cover observation photo-interpreted (and/or observed in the field) on a global scale. Thanks to an innovative method allowing to assess observer’s accuracy, this massive crowdsourced data can be used as training dataset for an automated land cover classification algorithm (SVM) of Landsat images. This near real time active learning method, to the best of our knowledge, is unique in the world.

{{< youtube F-XZ6b2Qxg8>}}

##METHOD

#THE SAMPLING

The most recent Landsat images are downloaded and sampled in objects of 9x9 pixels by stratified sampling. Strata are defined using the world map of Köppen−Geiger Climate Classes (figure 1), larger is the area of the classes (figure 2), the more units are sampled.



{{< figure src="/img/stratification.jpg" caption="World Map of Köppen−Geiger Climate Classification." >}}

#GAME RULES

The goal is to conquer as much territory (district, province, region) as possible and become the master of the World. To claim a territory, the user has to correctly identify the land cover of each sample units in it and complete several challenges (quiz, speed test, etc). Each new user starts with a dedicated game mode, the sandbox. During the sandbox phase, the accuracy of the gamer will be tested against a series of sample unit that have been preclassified based on expert knowledge. After this phase, a level of confidence (specified for each classes) will be given at each user. From that point,, the gamer will be able to choose territories he wants to explore. When a territory is discover for the first time, the explorer mode will be activated. This phase continues until each sample units of the territory have been assessed by 10 different users. When the phase is over, a “true” land cover is determined for each sample unit based on a weighting of the different answers (function of the level of confidence) and the last up-to-date land cover map. If the guess was right, the gamer marked a point. A territory is given at a user if he had an accuracy higher than 70%. When a territory has passed the explorer stage, it can be visited by any users, the “true” land cover of a sample unit can changed in time if the new weighted answer is different. In this case points are deducted to concerned gamers. The level of confidence of each users is also updated during the game depending on the number of his right answers. A territory is never definitively acquired. New sample units can appear in a zone already owned. In this case the territory is under siege (similar mechanisms than the explorer mode) until each new sample unit has been validated by 10 users or more.

Improved the gaming experience with several features: League, Badges, Special Challenge, Bet your territories…

#LAND COVER CLASSIFICATION

The sample units that have passed the explorer mode are used to train a Support Vector Machine algorithm in the stratum concerned. As the carry out of the validation data progresses, the best available land cover map is updated. When change are detected between successive land cover maps, the area will be submitted to users for validation. This kind of feedback from the users is, to the best of our knowledge, unique in the world.


