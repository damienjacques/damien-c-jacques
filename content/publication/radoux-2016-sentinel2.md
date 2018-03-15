+++
title = "Sentinel-2’s Potential for Sub-Pixel Landscape Feature Detection"
date = "2016-06-09"

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Julien Radoux", "Guillaume Chomé", "Damien C. Jacques", "François Waldner", "Nicolas Bellemans", "Nicolas Matton", "Céline Lamarche", "Raphaël d’Andrimont", "Pierre Defourny"]

# Publication type.
# Legend:
# 0 = Uncategorized
# 1 = Conference proceedings
# 2 = Journal
# 3 = Work in progress
# 4 = Technical report
# 5 = Book
# 6 = Book chapter
publication_types = ["2"]

# Publication name and optional abbreviated version.
publication = "*Remote Sensing*"
# publication_short = "In *ICMEW*"

# Abstract and optional shortened version.
abstract = "The ground truth data sets required to train supervised classifiers are usually collected as to maximize the number of samples under time, budget and accessibility constraints. Yet, the performance of machine learning classifiers is, among other factors, sensitive to the class proportions of the training set. In this letter, the joint effect of the number of calibration samples and the class proportions on the accuracy was systematically quantified using two state-of-the-art machine learning classifiers (random forests and support vector machines). The analysis was applied in the context of binary cropland classification and focused on two contrasted agricultural landscapes. Results showed that the classifiers were more sensitive to class proportions than to sample size, though sample size had to reach 2,000 pixels before its effect leveled off. Optimal accuracies were obtained when the training class proportions were close to those actually observed on the ground. Then, synthetic minority over-sampling technique (SMOTE) was implemented to artificially regenerate the native class proportions in the training set. This resampling method led to an increase of the accuracy of up to 30%. These results have direct implications for (i) informing data collection strategies and (ii) optimizing classification accuracy. Though derived for cropland mapping, the recommendations are generic to the problem of binary classification."

# Featured image thumbnail (optional)
image_preview = ""

# Is this a selected publication? (true/false)
selected = false

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter the filename (excluding '.md') of your project file in `content/project/`.
# projects = ["example-external-project"]

# Links (optional).
url_pdf = "http://www.mdpi.com/2072-4292/8/6/488/pdf"
# url_preprint = "#"
# url_code = "#"
# url_dataset = "#"
# url_project = "#"
# url_slides = "#"
# url_video = "#"
# url_poster = "#"
# url_source = "#"

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
url_custom = [{name = "Publisher Full Text", url = "http://www.mdpi.com/2072-4292/8/6/488"},
{name = "Altmetrics", url = "https://mdpi.altmetric.com/details/8605579/qa"}]

# Does the content use math formatting?
math = true

# Does the content use source code highlighting?
highlight = true

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
[header]
# image = "headers/bubbles-wide.jpg"
# caption = "My caption :smile:"

+++