---
permalink: /
title: #"academicpages is a ready-to-fork GitHub Pages template for academic personal websites"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

# Yicheng Ouyang
I am a third-year Computer Science PhD student at [University of Illinois Urbana-Champaign](https://cs.illinois.edu/) advised by Professor [Lingming Zhang](https://lingming.cs.illinois.edu/) and Professor [Darko Marinov](https://mir.cs.illinois.edu/marinov/). My research interest lies in Software Engineering, specifically Automated Program Repair, Fault Localization, Program Analysis and Software Testing. Before coming to UIUC, I completed my undergrad at the Southern University of Science and Technology where I was fortunate to work with Professor [Yuqun Zhang](https://zhangyuqun.github.io/).

## Publications
**MirrorTaint: Practical Non-intrusive Dynamic Taint Tracking for JVM-based Microservice Systems.**  
**Yicheng Ouyang**, Kailai Shao, Kunqiu Chen, Ruobing Shen, Chao Chen, Mingze Xu, Yuqun Zhang, Lingming Zhang.  
*In Proceedings of the 45th IEEE/ACM International Conference on Software Engineering ([ICSE 2023](https://conf.researchr.org/home/icse-2023))*, 2023. [[PDF](https://yicheng-ouyang.github.io/files/MirrorTaint.pdf)]

**SJFuzz: Seed \& Mutator Scheduling for JVM Fuzzing.**  
Mingyuan Wu, **Yicheng Ouyang**, Minghai Lu, Junjie Chen, Yingquan Zhao, Heming Cui, Guowei Yang, Yuqun Zhang.  
*In Proceedings of the 31st ACM Joint European Software Engineering Conference and Symposium on the Foundations of Software Engineering ([FSE 2023](https://2023.esec-fse.org/))*, 2023. [[PDF](https://yicheng-ouyang.github.io/files/SJFuzz.pdf)]

**Fast and Precise On-the-fly Patch Validation for All.**  
Lingchao Chen, **Yicheng Ouyang**, Lingming Zhang.  
*In Proceedings of the 43rd IEEE/ACM International Conference on Software Engineering ([ICSE 2021](https://conf.researchr.org/home/icse-2021))*, 2021. [[PDF](https://yicheng-ouyang.github.io/files/UniAPR.pdf)]

**Simulee: Detecting CUDA Synchronization Bugs via Memory-Access Modeling.**  
Mingyuan Wu, **Yicheng Ouyang**, Husheng Zhou, Lingming Zhang, Cong Liu, Yuqun Zhang.  
*In Proceedings of the 42nd IEEE/ACM International Conference on Software Engineering ([ICSE 2020](https://conf.researchr.org/home/icse-2020))*, 2020. [[PDF](https://yicheng-ouyang.github.io/files/Simulee.pdf)]

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the academicpages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring academicpages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
