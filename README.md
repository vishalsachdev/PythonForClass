# Python for Class 

A 'How to ' Guide for using python/Jupyter notebooks for class. 
Includes an overview of common tools to run python/jupyter on your computer and on the cloud. This is prepared for teachers interested in using the tools for teaching and not for production /deployment, directed at teachers outside the CS domain. I will also cover options for integrating with LMS. I teach in the GIES College of business at UIUC and am preparing this for faculty here purely for the purpose of making a decision on the platform  and the tools. No discussion on learning python or any algorithms itself. This guide assumes that the front end will always be a jupyter notebook and you are using python 3 for the analysis. 



## On device or on the cloud 
On device installs are clearly a good option for saving cloud hosting costs, and force students to learn how to setup a local environment for their work. Most beginner student projects dont involve big data sets, so most devices should be able to run python. However, if it is a large class, and typically 10% of your students will have trouble with installs, and you dont have a TA, you should plan on sending some time in the first two sessions doing trouble shooting. This luxury of time is typically possible only for 16 week courses.   No trouble shooting/no hardware/software constraints on students. If there is no pedagogical justification for having students learn how to manage on device analytics backend and you can afford it, go for an on cloud solution. For a large class (> 50 students), go for a paid cloud solution or find a free cloud solution. On the other hand, for masters students, I would almost always recommend on cloud, unless they expect to do research or do intensive analytics, where cloud can become expensive. 

My recommendation 
- Undergraduate semester long beginner classes - On device (if pedagogical need or no budget), else on cloud
- Short term/ graduate courses- On cloud (saves time) 

## On Device  
When choosing on device , you want to pick a package manager which is essential to download/update the packages needed for analysis. For python, you have two basic options - Just install a package manager, Conda with some other libraries( miniconda https://docs.conda.io/en/latest/miniconda.html ) OR  install a manager along with many default packages(Anaconda - Big download 3 GB https://www.anaconda.com/distribution/ ). My recommendation- Go with miniconda and then have students install the packages they need, as the semester progresses. Less setup time, and teaches students how to get packages for their needs. A detailed comparison can be found at [anaconda-vs-miniconda] (http://deeplearning.lipingyang.org/2018/12/23/anaconda-vs-miniconda-vs-virtualenv/)

My recommendation- Go with miniconda and then have students install the packages they need. 

## On Cloud 
- Free
Good for shorter projects, and some offer team collaboration features. Several free Google and Microsoft and others. One of the best comparison of six free options, is at https://www.dataschool.io/cloud-services-for-jupyter-notebook/ . From my perspective, the most important criteria is that the free option should be the following 
1. compatible or portable to an on device install or another cloud providers( Kaggle fails here, but it is a great option)
2. reasonable memory/disk space 

Wishlist 
1. pure jupyter experience 
2. One click deployment of code as interactive notebooks (mybinder, Google Collab ) - useful for quick start and short workshops. 
3. LMS integration 



- Paid 




You can use the [editor on GitHub](https://github.com/vishalsachdev/PythonForClass/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

