# A 'How to ' Guide for using python/Jupyter notebooks for class
View web ready version at https://vishalsachdev.github.io/python4class/

This guide gives an overview of common tools to run python/jupyter on your computer and on the cloud. This is prepared for teachers interested in using the tools for teaching and not for production /deployment and directed at teachers outside the CS domain. I will also cover options for integrating with LMS. I teach in the GIES College of business at UIUC and am preparing this for faculty here purely for the purpose of making a decision on the platform  and the tools. No discussion on learning python or any algorithms itself. This guide assumes that the front end will always be a jupyter notebook and you are using python 3 for the analysis.



## On device or on the cloud
On device installs are clearly a good option for saving cloud hosting costs, and force students to learn how to setup a local environment for their work. Most beginner student projects dont involve big data sets, so most devices should be able to run python. However, if it is a large class, and typically 10% of your students will have trouble with installs, and you dont have a TA, you should plan on sending some time in the first two sessions doing trouble shooting. This luxury of time is typically possible only for 16 week courses.   No trouble shooting/no hardware/software constraints on students. If there is no pedagogical justification for having students learn how to manage on device analytics backend and you can afford it, go for an on cloud solution. For a large class (> 50 students), go for a paid cloud solution or find a free cloud solution. On the other hand, for masters students, I would almost always recommend on cloud, unless they expect to do research or do intensive analytics, where cloud can become expensive.

My recommendation
- Undergraduate semester long beginner classes - On device (if pedagogical need or no budget), else on cloud
- Short term/ graduate courses- On cloud (saves time)

## On Device  
When choosing on device , you want to pick a package manager which is essential to download/update the packages needed for analysis. For python, you have two basic options - Just install a package manager, Conda with some other libraries( [miniconda](https://docs.conda.io/en/latest/miniconda.html) ) OR  install a manager along with many default packages([Anaconda](https://www.anaconda.com/distribution/) - Big download 3 GB  ). My recommendation- Go with miniconda and then have students install the packages they need, as the semester progresses. Less setup time, and teaches students how to get packages for their needs. A detailed comparison can be found at [anaconda-vs-miniconda](http://deeplearning.lipingyang.org/2018/12/23/anaconda-vs-miniconda-vs-virtualenv/)

My recommendation- Go with miniconda and then have students install the packages they need.

## On Cloud
- Free
Good for shorter projects, and some offer team collaboration features. Several free Google and Microsoft and others. One of the best comparison of six free options, is at [dataschool.io](https://www.dataschool.io/cloud-services-for-jupyter-notebook/) . From my perspective, the most important criteria for the free option should be the following

1. The Cloud interface should either be a pure open source experience(or close enough), so that students can transfer that learning on to their own installs on device. If the interface is significantly different, it should allow for a python notebook download . Kaggle fails here, but it is a great option. Some platforms for learning python, such as Dataquest.io, allow for a python notebook export.
2. Reasonable memory for processing and disk space for data


My Recommendation
- For short modules (couple of weeks)- Use [Google Colab](https://colab.research.google.com/), which is also well integrated with github. There is a [chrome extension](https://chrome.google.com/webstore/detail/open-in-colab/iogfkhleblhcpcekbiedikdehleodpjo?hl=en)  as well, for opening any notebook on github, on Colab with one click. CoLab has a generous compute/memory/storage allocation. If you prefer the Microsoft stack, try [Azure](https://notebooks.azure.com/).
- For one off demo activity - Students dont need to get into code much. Cookbook approach. Go with hosting the notebook on github and use [MyBinder](https://ovh.mybinder.org/) for creating an interactive notebook. If you want to give it some interactivity, add an extension
- For semester long courses- Review paid options below.


- Paid
Since the software is open source, you will pay either for for hosting the notebooks(compute and data storage) on any cloud provider such as Microsoft, Google, or Amazon or you might pay for a full featured solution, where you get hosting/compute and an autograder with LTI integration into the Learning Management System.

1. Hosted Jupyter Notebook on any cloud provider - UIUC has a contract with cloud providers such as Amazon and Microsoft, and most schools would have some similar contracts. Some of these vendors offer custom/optimized jupyter hosted solutions ([amazon](https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-managed-notebooks.html)) .

2. LMS integration- Most LMS these days offer LTI integration, and opening Jupyter notebooks within an LMS is a trivial activity, and there are paid options, such as [illumidesk](https://www.illumidesk.com/) (specific for Canvas). What would be ideal is to have an autograder do the grading, if you have large classes. We used a cloud provider (https://www.vocareum.com/)  over the past 6 months with a few faculty for a 600 student intro analytics course. This platform provides LMS integration, clould hosting and autograding. The ability to have sophomores get started with python/jupyter with no setup time was great. We saved a lot of troubleshooting time, and the autograding saved a lot of time. You still have to code the autograding scripts and learn the platform, which is a sunk cost.  Do note that if you are the DIY techie, or have dedicated IT support, you could do LTI integration by yourself, and use an open source [autograding solution](https://github.com/jupyter/nbgrader) , with helpful information at [gryd.us](https://gryd.us/autograding-using-jupyter-notebooks/).

My Recommendation- For business school faculty, who would rather go for a self-service approach, a paid hosted solution with a LMS integration with autograding would be the ideal option. 

This writeup focuses on hosting notebooks, but if you want help in the pedagogy around using jupyter notebooks in class, along with some help on hosting, I highly recommend a free e-book created by a group of faculty during a conference and updated often after that at [jupyter4edu](https://jupyter4edu.github.io/jupyter-edu-book/)
