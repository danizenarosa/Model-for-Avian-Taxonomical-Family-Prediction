# dsci-100-project_template
Template project repository for DSCI-100

project creation date: Feb 8th, 2024


Introduction:

Birdwatching, and associated activities such as identifying birds, has been a common hobby for centuries. In just February of this year, the world record for most birds having been seen across the world, 10 000 birds, was broken. A new bird species, the Cinnyris infrenatus, was found as recently as 2022 and there will never be a guarantee that humans have identified all bird species. If non-experts come across a bird which happens to be an unknown species, the only form of evidence they might be able to collect  may be a picture. From these pictures we would likely be able to identify dimensions such as the bird's wingspan, beak size and more. 

Thus, our question is:
Based on a set of given bird's dimensions, what family can we predict this bird belongs to?

We will be using the AVONET database, compiled by Tobias et al. (2022). It is compiled in an excel sheet. We will primarily be focusing on page 2 of the excel sheet "AVONET1_BirdLife". This dataset describes more than 90 000 individual birds from over 11 000 species. The individuals are grouped into species and each observation includes the order and family of each species of bird as well as the average beak length, width and depth, wingspan, tarsus length, kipps distance, tail length and mass among all recorded individuals of the species. There is also location information in the form of the average coordinates at which the birds were found as well as the habitat in which they inhabited. 

Tobias, J. A., Sheard, C., Pigot, A. L., Devenish, A. J., Yang, J., Sayol, F., Neate‐Clegg, M. H., Alioravainen, N., Weeks, T. L., Barber, R. A., Walkden, P. A., MacGregor, H. E., Jones, S. E., Vincent, C., Phillips, A. G., Marples, N. M., Montaño‐Centellas, F. A., Leandro‐Silva, V., Claramunt, S., … Schleuning, M. (2022). Avonet: Morphological, ecological and geographical data for all birds. Ecology Letters, 25(3), 571–707. https://doi.org/10.1111/ele.13898 

Preliminary exploratory data analysis:


Methods: 

In this investigation, we will be using the columns; beak length, beak width, beak depth, tarsus length, wing length, kipps distance, hand-wing index, tail length and mass as the dimensions of the bird to classify the family that the invdividual belongs in. We will perform cross-validation to evaluate the performance of the model and to identify the k nearest neighbors value that best reflects the whole dataset. One way that we will visualize the results is through a set of plots that contain specific characterstics and their resulting families, for example, beak length vs family.



Expected outcomes and significance:

We expect to find a strong correlation between bird dimensions and their family, even across different species. Should the dimensions themselves not have strong correlation with their families, we expect the ratios of these dimensions should also show a strong relationship between species of the same family. From this we will be able to predict the family of unknown birds based only on their dimensions. 
If non-experts come across new bird species, it could be vital to be able to identify the bird's close biological relatives (i.e the bird's family on the tree of life) for scientists to identify important biological traits without being present to study them. As mentioned above, it is likely evidence will only be able to exist in the form of an image and so more specific behavioural data may not be able to be taken. 
If our hypothesis is proven, then it could lead to questions about how or why certain species, despite living on opposite sides of the world, develop similar characteristics.