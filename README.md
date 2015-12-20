Topic Models Learning and R Resources
============


This is a collection documenting the resources I find related to topic
models with an R flavored focus. A *topic model* is a type of
[*generative*](https://en.wikipedia.org/wiki/Generative_model) model
used to "discover" latent topics that compose a *corpus* or collection
of documents. Typically topic modeling is used on a collection of text
documents but can be used for other modes including use a caption
generation for images.

![](inst/figure/topic-model.jpg)


Table of Contents
============

-   [Key Players](#key-players)
-   [Videos](#videos)
    -   [Introductory](#introductory)
    -   [Theory](#theory)
    -   [Visualization](#visualization)
-   [blob/master/articles](#blobmasterarticles)
-   [Websites & Blogs](#websites--blogs)
-   [R Resources](#r-resources)
    -   [Package Comparisons](#package-comparisons)
    -   [References](#references)
-   [Topic Modeling R Demo](#topic-modeling-r-demo)
    -   [Install/Load Tools & Data](#installload-tools--data)
    -   [Generate Stopwords](#generate-stopwords)
    -   [Create the DocumentTermMatrix](#create-the-documenttermmatrix)
    -   [Run the Model](#run-the-model)
    -   [Plot the Topics Per Person & Time](#plot-the-topics-per-person--time)
    -   [LDAvis of Model](#ldavis-of-model)
-   [Contributing](#contributing)

Key Players
============


Papadimitriou, Raghavan, Tamaki & Vempala, Santosh (1997) first
introduced the notion of topic modeling in their ["Latent Semantic
Indexing: A probabilistic
analysis"](blob/master/articles/Papadimitriou1997.pdf). Thomas Hofmann
(1999) developed "Probabilistic latent semantic indexing". Blei, Ng, &
Jordan (2003) proposed *latent Dirichlet allocation* (LDA) as a means of
modeling documents with multiple topics but assumes the topic are
uncorrelated. Blei & Lafferty (2007) proposed *correlated topics model*
(CTM), extending LDA to allow for correlations between topics. Roberts,
Stewart, Tingley, & Airoldi (2013) propose a [*Structural Topic
Model*](blob/master/articles/Roberts2013.pdf) (STM), allowing the
inclusion of meta-data in the modeling process.

Videos
======

Introductory
------------

-   Boyd-Graber, J. (2013). [Computational Linguistics I: Topic
    Modeling](https://www.youtube.com/watch?v=4p9MSJy761Y)

Theory
------

-   Blei, D. (2007) [Modeling Science: Dynamic Topic Models of Scholarly
    Research](https://www.youtube.com/watch?v=7BMsuyBPx90)

-   Blei, D. (2009) [Topic Models: Parts I &
    II](http://videolectures.net/mlss09uk_blei_tm/#) ([Lecture
    Notes](blob/master/presentations/Blei2009.pdf))

Visualization
-------------

-   statgraphics (2014) [LDAvis: A method for visualizing and
    interpreting topic
    models](https://www.youtube.com/watch?v=IksL96ls4o0)

blob/master/articles
====================

-   Blei, D. M. (2012). [Probabilistic topic
    models](blob/master/articles/Blei2012.pdf). *Communications of the
    ACM, (55)*4, 77-84. DOI: 10.1145/2133806.2133826

-   Blei, D. M. & Lafferty, J. D. (2007) [A correlated topic model of
    Science](blob/master/articles/Blei2007.pdf). *The Annals of Applied
    Statistics 1*(1), 17-35. <doi:10.1214/07-AOAS114>.
    <http://projecteuclid.org/euclid.aoas/1183143727>.

-   Blei, D. M. & Lafferty, J. D. (2009) [Topic
    models](blob/master/articles/Blei2009.pdf). In A Srivastava, M
    Sahami (eds.), [*Text mining: classification, clustering, and
    applications*](blob/master/articles/Srivastava2009.pdf). Chapman &
    Hall/CRC Press. 71-93.

-   Blei, D. M. & McAuliffe, J. (2008). [Supervised topic
    models](blob/master/articles/Blei2008.pdf). In Advances in Neural
    Information Processing Systems 20. 1-8.

-   Blei, D. M., Ng, A.Y., & Jordan, M.I. (2003). [Latent Dirichlet
    Allocation](blob/master/articles/Blei2003.pdf). *Journal of Machine
    Learning Research, 3*, 993-1022.

-   Chang, J., Boyd-Graber, J. , Wang, C., Gerrish, S., & Blei. D.
    (2009). [Reading tea leaves: How humans interpret topic
    models](blob/master/articles/Chang2009.pdf). In *Neural Information
    Processing Systems*.

-   Griffiths, T.L. & Steyvers, M. (2004). [Finding Scientific
    Topics](blob/master/articles/Griffiths2004.pdf). Proceedings of the
    National Academy of Sciences of the United States of America, 101,
    5228-5235.

-   Grüen, B. & Hornik, K. (2011). [topicmodels: An R Package for
    Fitting Topic Models. Journal of Statistical
    Software](blob/master/articles/Grun2011.pdf), 40(13), 1-30.

-   Roberts M.E., Stewart B.M., Tingley D., & Airoldi E.M. (2013) [The
    Structural Topic Model and Applied Social
    Science](blob/master/articles/Roberts2013.pdf). *Advances in Neural
    Information Processing Systems Workshop on Topic Models:
    Computation, Application, and Evaluation*. 2013.

-   Roberts, M., Stewart, B., Tingley, D., Lucas, C., Leder-Luis, J.,
    Gadarian, S., Albertson, B., et al. (2014). [Structural topic models
    for open ended survey
    responses](blob/master/articles/Roberts2014.pdf). *American Journal
    of Political Science, American Journal of Political Science, 58*(4),
    1064-1082.

-   Roberts, M., Stewart, B., Tingley, D. (n.d.). [stm: R Package for
    Structural Topic Models](blob/master/articles/Robertsnd.pdf), 1-49.

-   Sievert, C. & Shirley, K. E.. (2014). [LDAvis: A Method for
    Visualizing and Interpreting
    Topics.](blob/master/articles/Robertsnd.pdf) *Proceedings of the
    Workshop on Interactive Language Learning, Visualization, and
    Interfaces* 63-70.

Websites & Blogs
================

-   Blei, D. (nd). [David Blei on Topic
    Models](https://www.cs.princeton.edu/~blei/topicmodeling.html)

-   Jockers, M.L. (2013). ["Secret" Recipe for Topic Modeling
    Themes](http://www.matthewjockers.net/2013/04/12/secret-recipe-for-topic-modeling-themes/)

-   Schmidt, B.M. (20) [Words Alone: Dismantling Topic Models in the
    Humanities](http://journalofdigitalhumanities.org/2-1/words-alone-by-benjamin-m-schmidt/)

-   Weingart, S. (2012). [Topic Modeling for Humanists: A Guided
    Tour](http://www.scottbot.net/HIAL/?p=19113)

R Resources
===========

Package Comparisons
-------------------

<table>
<thead>
<tr class="header">
<th align="left">package</th>
<th align="left">function</th>
<th align="left">pluses</th>
<th align="left">author</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left">lda</td>
<td align="left">Collapsed Gibbs for LDA</td>
<td align="left"></td>
<td align="left">Chang</td>
</tr>
<tr class="even">
<td align="left">topicmodels</td>
<td align="left">LDA and CTM</td>
<td align="left">Follows Blei's implementation; great vignette; takes <a href="https://en.wikipedia.org/wiki/Document-term_matrix">DTM</a></td>
<td align="left">Grüen &amp; Hornik</td>
</tr>
<tr class="odd">
<td align="left">stm</td>
<td align="left">Model w/ meta-data</td>
<td align="left">Great documentation; nice visualization</td>
<td align="left">Roberts, Stewart, &amp; Tingley</td>
</tr>
<tr class="even">
<td align="left">LDAvis</td>
<td align="left">Interactive visualization</td>
<td align="left">Aids in model interpretation</td>
<td align="left">Sievert &amp; Shirley</td>
</tr>
</tbody>
</table>

References
----------

-   Chang J. (2010). lda: Collapsed Gibbs Sampling Methods for Topic
    Models. R package version 1.2.3, URL
    <http://CRAN.R-project.org/package=lda>.

-   Grüen, B. & Hornik, K. (2011). [topicmodels: An R Package for
    Fitting Topic Models. Journal of Statistical
    Software](blob/master/articles/Grun2011.pdf), 40(13), 1-30.

-   Roberts, M., Stewart, B., Tingley, D. (n.d.). [stm: R Package for
    Structural Topic Models](blob/master/articles/Robertsnd.pdf), 1-49.

-   Sievert, C. & Shirley, K. E.. (2014). [LDAvis: A Method for
    Visualizing and Interpreting
    Topics.](blob/master/articles/Robertsnd.pdf) *Proceedings of the
    Workshop on Interactive Language Learning, Visualization, and
    Interfaces* 63-70.

Topic Modeling R Demo
=====================

The .R script for this demonstration can be downloaded from
[scripts/Example\_topic\_model\_analysis.R](https://raw.githubusercontent.com/trinker/topicmodels_learning/master/scripts/Example_topic_model_analysis.R)

Install/Load Tools & Data
-------------------------

    if (!require("pacman")) install.packages("pacman")
    pacman::p_load_gh("trinker/gofastr")
    pacman::p_load(tm, topicmodels, dplyr, tidyr,  devtools, LDAvis, ggplot2)

    ## Source topicmodels2LDAvis function
    devtools::source_url("https://gist.githubusercontent.com/trinker/477d7ae65ff6ca73cace/raw/79dbc9d64b17c3c8befde2436fdeb8ec2124b07b/topicmodels2LDAvis")

    ## SHA-1 hash of file is f9a066b61c9f992daff3991a3293e18897268598

    data(presidential_debates_2012)

Generate Stopwords
------------------

    stops <- c(
            tm::stopwords("english"),
            "governor", "president", "mister", "obama","romney"
        ) %>%
        gofastr::prep_stopwords() 

Create the DocumentTermMatrix
-----------------------------

    doc_term_mat <- presidential_debates_2012 %>%
        with(gofastr::q_dtm_stem(dialogue, paste(person, time, sep = "_"))) %>%           
        gofastr::remove_stopwords(stops) %>%                                                    
        gofastr::filter_tf_idf() %>%
        gofastr::filter_documents() 

Run the Model
-------------

    lda_model <- topicmodels::LDA(doc_term_mat, 10, control = list(seed=100))

Plot the Topics Per Person & Time
---------------------------------

    topics <- topicmodels::posterior(lda_model, doc_term_mat)[["topics"]]
    topic_dat <- dplyr::add_rownames(as.data.frame(topics), "Person_Time")
    colnames(topic_dat)[-1] <- apply(terms(lda_model, 10), 2, paste, collapse = ", ")

    tidyr::gather(topic_dat, Topic, Proportion, -c(Person_Time)) %>%
        tidyr::separate(Person_Time, c("Person", "Time"), sep = "_") %>%
        dplyr::mutate(Person = factor(Person, 
            levels = c("OBAMA", "ROMNEY", "LEHRER", "SCHIEFFER", "CROWLEY", "QUESTION" ))
        ) %>%
        ggplot2::ggplot(ggplot2::aes(weight=Proportion, x=Topic, fill=Topic)) +
            ggplot2::geom_bar() +
            ggplot2::coord_flip() +
            ggplot2::facet_grid(Person~Time) +
            ggplot2::guides(fill=FALSE) +
            ggplot2::xlab("Proportion")

![](inst/figure/unnamed-chunk-6-1.png)

LDAvis of Model
---------------

The output from **LDAvis** is not easily embedded within an R markdown
document, however, the reader may [see the results
here](http://trinker.github.io/LDAvis/example/).

    lda_model %>%
        topicmodels2LDAvis() %>%
        LDAvis::serVis()

Contributing
============

You are welcome to: 
* submit suggestions and bug-reports at: <https://github.com/trinker/topicmodels_learning/issues> 
* send a pull request on: <https://github.com/trinker/topicmodels_learning/> 
* compose a friendly e-mail to: <tyler.rinker@gmail.com>
