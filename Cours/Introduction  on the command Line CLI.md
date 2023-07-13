

# Introduction  on the command Line CLI

# Project Organization

## OVERVIEW

### Questions

- How can I organize my file system for a new bioinformatics project?
- How can I document my work?

### Objectives

- Create a file system for a bioinformatics project.
- Explain what types of files should go in your `docs`, `data`, and `results` directories.
- Use the `history` command and a text editor like `nano` to document your work on your project.

## Getting your project started

------

Project organization is one of the most important parts of a sequencing project, and yet is often overlooked amidst the excitement of getting a first look at new data. Of course, while it’s best to get yourself organized before you even begin your analyses, it’s never too late to start, either.

You should approach your sequencing project similarly to how you do a biological experiment and this ideally begins with experimental design. We’re going to assume that you’ve already designed a beautiful sequencing experiment to address your biological question, collected appropriate samples, and that you have enough statistical power to answer the questions you’re interested in asking. These steps are all incredibly important, but beyond the scope of our course. For all of those steps (collecting specimens, extracting DNA, prepping your samples) you’ve likely kept a lab notebook that details how and why you did each step. However, the process of documentation doesn’t stop at the sequencer!

Genomics projects can quickly accumulate hundreds of files across tens of folders. Every computational analysis you perform over the course of your project is going to create many files, which can especially become a problem when you’ll inevitably want to run some of those analyses again. For instance, you might have made significant headway into your project, but then have to remember the PCR conditions you used to create your sequencing library months prior.

Other questions might arise along the way:

- What were your best alignment results?
- Which folder were they in: Analysis1, AnalysisRedone, or AnalysisRedone2?
- Which quality cutoff did you use?
- What version of a given program did you implement your analysis in?

Good documentation is key to avoiding this issue, and luckily enough, recording your computational experiments is even easier than recording lab data. Copy/Paste will become your best friend, sensible file names will make your analysis understandable by you and your collaborators, and writing the methods section for your next paper will be easy! Remember that in any given project of yours, it’s worthwhile to consider a future version of yourself as an entirely separate collaborator. The better your documenation is, the more this ‘collaborator’ will feel indebted to you!

With this in mind, let’s have a look at the best practices for documenting your genomics project. Your future self will thank you.

In this exercise we will setup a file system for the project we will be working on during this workshop.

We will start by creating a directory that we can use for the rest of the workshop. First navigate to your home directory. Then confirm that you are in the correct directory using the `pwd` command.



````bash
$ cd
$ pwd
````

### EXERCISE

Use the `mkdir` command to make the following directories:

- `R_workshop`
- `R_workshop/docs`
- `R_workshop/data`
- `R_workshop/results`

Use `ls -R` to verify that you have created these directories. The `-R` option for `ls` stands for recursive. This option causes `ls` to return the contents of each subdirectory within the directory iteratively.

````bash
$ ls -R dc_workshop
````

