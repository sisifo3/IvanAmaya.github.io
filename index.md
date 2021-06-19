$if(mathjax)$
<!--- MathJax stuff -->
<script type="text/javascript" src='https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML'></script>
<script type="text/x-mathjax-config">
    MathJax.Hub.Config({ TeX: { equationNumbers: {autoNumber: "all"} } });
</script>
$endif$

## Artificial Intelligence.

In this space we will address issues related to Artificial Intelligence, in the book Artificial Intelligence a Modern Approach, written by Staiart Russell and Peter Norving divides the concepts into four possible areas such as: Systems that think like humans, Systems that think rationally, systems that acts like humans, systems that act rationally.[1]

[comment]: <> (You can use the)

[comment]: <> ([editor on GitHub](https://github.com/sisifo3/IvanAmaya.github.io/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.))

[comment]: <> (Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.)

### Machine Learning

[comment]: <> (Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for)


<details open>
<summary> Occurence Probability</summary>

<p>The approach to data analysis is based on the mean of the distribution represented by the next equation, which is the standard form of the Gaussian distribution [2]. 
  
    \begin{equation}  
P(x) = \frac{1}{\sqrt{2 \pi \sigma ^2}} e^{\frac{x - \mu }{2 \sigma ^2}}
\end{equation}    

Where $P(x)$ is the probability of occurrence of the variable n, $\sigma$ is the Standard deviation, $\sigma$ 2 is the Variance, $\mu$ is the Mean. The method is based on the postulate that the values of the unknown parameters are those that produce a maximum probability of observing the measured data. Assuming
that the measurements are independent of each other [2]. <br/>

    
  </p>
</details>  

Data distribution 

If we want to plot a data <br/>

  

```markdown
library(ggplot2)
#Name     label  
#Control  <- 0 
#ADHD     <- 1    

file1 <-"Desktop/Ingoodwetrust/libros/ADHD_dataset_2/var_st_entropy_AP_RP_Control_ADHD_V2_1.csv"
df1 <- read.csv(file1)

file0 <-"Desktop/Ingoodwetrust/libros/ADHD_dataset_2/var_st_entropy_AP_RP_Control_ADHD_V2_0.csv"
df0 <- read.csv(file0)

g1 <- replicate(265,"ADHD")
g2<- replicate(265,"Control")

df1$group <- g1 
df0$group <- g2
df <- rbind(df1,df0)

df$Entropy <- df$entropy

p2 <- ggplot(df, aes(x=Entropy, fill=group, binwidth=.3)) + geom_density(col = "green", alpha=.6) 

p2

```



![alt text for screen readers](/path/to/image.png "Text to show on mouseover")



<img src="/assets/img/MarineGEO_logo.png" alt="MarineGEO circle logo" style="height: 100px; width:100px;"/>


<details open>
<summary> Linear Regression</summary>

<p>
The simple linear regression model, is a model with a single regressor x that has a relationship with a response y that is a straight line, we can found this
equations in the book Introduction to linear regression Analysis [3].

    \begin{equation}  
y_0 = \beta_0 + \beta_1 x_0
\end{equation}    
 
where the intercept $\beta_0$ and the slope $\beta_1$ are unknown constants.
    
  </p>
</details>  









[comment]: <> (For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).)

[comment]: <> (### Jekyll Themes)

[comment]: <> (Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/sisifo3/IvanAmaya.github.io/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.)

[comment]: <> (### Support or Contact)

[comment]: <> (Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.)


### References.

[1] Stuart Russel, Peter Norving . (2004). Artificial Intelligence a Modern Approach. 28042 Madrid (España): Pearson Education,.

[2] M. Bonamente, Statistics and Analysis of Scientific Data. Springer Science+Business Media New York 2013, 2013.

[3] Douglas C. Montgomery. (2012). Introduction to Linear Regression Analysis. Hoboken, New Jersey.: John Wiley & Sons, Inc




$if(mathjax)$
<!--- MathJax stuff -->
<script type="text/javascript" src='https://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML'></script>
<script type="text/x-mathjax-config">
    MathJax.Hub.Config({ TeX: { equationNumbers: {autoNumber: "all"} } });
</script>
$endif$

