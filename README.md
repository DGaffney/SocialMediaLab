# SocialMediaLab

Note: if you are getting the error `Error in check_twitter_oauth( )`, please find a [solution here](https://github.com/geoffjentry/twitteR/issues/90).

`SocialMediaLab` is an R package that provides a suite of tools for collecting and constructing networks from social media data. It provides easy-to-use functions for collecting data across popular platforms (Instagram, Facebook, Twitter, and YouTube) and generating different types of networks for analysis.

SocialMediaLab was created by [Timothy Graham](http://uq.academia.edu/TimGraham) (who is also the maintainer of the package) and [Robert Ackland](https://researchers.anu.edu.au/researchers/ackland-rj).

The latest 'official' version of the package can also be found on [CRAN](https://cran.r-project.org/web/packages/SocialMediaLab/index.html).

This package would not be possible without key packages by other authors in the R community, particularly: [igraph](https://github.com/igraph/rigraph), [Rfacebook](https://github.com/pablobarbera/Rfacebook), [instaR](https://github.com/pablobarbera/instaR), [twitteR](https://github.com/geoffjentry/twitteR), [data.table](https://github.com/Rdatatable/data.table), [tm](https://cran.r-project.org/web/packages/tm/index.html), and [httr](https://github.com/hadley/httr).

## Getting started

For detailed information and examples, please refer to the [SocialMediaLab documentation](https://github.com/voson-lab/SocialMediaLab/blob/master/SocialMediaLab.pdf).

The [SocialMediaLab page on the VOSON website](http://voson.anu.edu.au/SocialMediaLab) also has several "how to" guides, including an "Absolute Beginners Guide to SocialMediaLab" tutorial aimed at people with little or no programming experience.

## Example networks

The following networks were created in SocialMediaLab and visualised using the [Gephi software](http://gephi.github.io/).

##### Facebook bimodal network (Star Wars page)

This network visualises two weeks of activity on the [Star Wars Facebook page](https://www.facebook.com/StarWarsAUNZ/?brand_redir=169299103121699). Nodes (vertices) represent either users or posts, and node ties (edges) represent either 'likes' or comments. Nodes are sized by out-degree and coloured by modularity cluster.

<img src="http://voson.anu.edu.au//papers/ACSPRIWinter2015/Facebook_bimodal_network_socialmedialab_Star_Wars.png" alt="Facebook bimodal network created with SocialMediaLab" width="600" height="600"/>

##### Instagram ego network

This network visualises the social network of one user (the 'ego' node) on Instagram. The degree of the network is "2", meaning that it shows *ego + alters* ("followers of ego") and *ego + alters* + *alters of alters of ego* "followers of followers of ego". 'Follows' data are also collected, so this network also shows "users who ego follows" and "users who followers of ego follow".

<img src="http://voson.anu.edu.au//papers/ACSPRIWinter2015/Instagram_ego_network_socialmedialab_example.png" alt="Facebook bimodal network created with SocialMediaLab" width="600" height="600"/>

