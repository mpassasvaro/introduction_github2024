# Repository management and collaborative science platforms:  GitHub

*Objectives of this session:*

- To create a repository and include the basic information.
- To know in detail the version history of the repository.
- To manage and compare the versions of the files in the repository.
- To manage different branches for a repository.
- To know what are fork and pull request on repositories.
- To collaborate and to share with other members in a repository.
- To learn about other features to improve the work with repositories.

**Table of contents**
<HR>

<!-- vscode-markdown-toc -->

Exercises  
- [Exercise 1 - Create an initial repository. Commits and history](#exercise1-init-repo)
- [Exercise 2 - Plan your work: Issues](#exercise2-issues)
- [Exercise 3 - How to manage branches and Pull Requests](#exercise3-branches-pr)
- [Exercise 4 - Collaborate in a repo. Fork a repository](#exercise4-collaborate-fork)

<!-- vscode-markdown-toc-config
	numbering=true
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->

<HR>

# <a name='exercise1-init-repo'></a>Exercise 1 - Create an initial repository for this session

:pill: **Aim of this exercise**
In this exercise a new repository will be created and some modifications and data files will be added. Finally, the history of changes made will be reviewed.

<HR>

### 1.1 Create a repository

For this training exercise it will be necessary to create a new repository with the following initial details: 

- Repository name: ``github-training``.
- Repository description: ``Repository for the exercise 1``.
- Repository scope: ``Public``.
- Licence: For example select the ``MIT licence``.
- Add a default ``README.md``.

In the following image you can see the options to select for the creation of the repository:

 ![exercise example 1](./media/exercise1.1.png)

Add some information to your repository by modyfing the `README.md` file. Use the following text to update the `README.md` file.

```
## SO-IAA training course: Introduction to Github

This is the working repository for the course exercises.
This repository will be used to practise commits, issues, branching and pull requests. 

# Session 1

## Creating a new repository and adding content

- [ ] Created repository
- [ ] Updated content

```
:arrow_right: Commit the change

### 1.2 Populate the repository with e data table

Once the README is ready, add the following data file named `power.csv`, copying and pasting the following content:

```
date,max,avg,min
2021-10-05 15:00,5285.0,4126.0,3968.0
2021-10-05 15:15,5292.0,4125.0,3953.0
2021-10-05 15:30,5296.0,4125.0,3950.0
```

:arrow_right: Commit the change

Once this change is made, add a couple more lines of data to the `power.csv` file:

```
2021-10-05 15:45,5287.0,4123.0,3952.0
2021-10-05 16:00,5234.0,4122.0,3965.0
```
:arrow_right: Commit the change

:checkered_flag: :checkered_flag: After these steps, you can check the version history. 
> Could you go back to a previous version of the data table?

# <a name='exercise2-issues'></a>Exercise 2 - Plan and manage your work: Issues

### 2.1 Create a text file and populate a list of Github Issues

:arrow_right: Create a file named `observations.txt`. Fill it with these contents:

```
Target Name      Instrument       Frequency (GHz)    Sensitivity (μJy)
NGC 4321         VLA             1.4                                60
M87              ALMA                            230                
NGC 6946         MeerKAT         1.4              15               
M51              VLA             3.0                                
Andromeda        GMRT            0.325            100              
NGC 253          ALMA                            115                
```

:arrow_right: Create the following issues and add the descriptions below to them:

**Issue 1: Missing sensitivity for M87**

> The Sensitivity value for M87 is missing. Add 2.5 μJy.

**Issue 2: Empty frequency for NGC 253**

> The Frequency value for NGC 253 is missing. Add 115 GHz.

**Issue 3: Fix sensitivity for M51**

> The Sensitivity value for M51 is missing. Add 5 μJy.

**Issue 4: Fix frequency for M87**

> The Frequency value for M87 is missing. Add 230 GHz.

**Issue 5: Align table formatting**

> The table has inconsistent spacing. Reformat it for proper alignment.

Once the issues are created, make sure to assign yourself to them and continue with the exercise.

:bulb: If you want, you can define a Milestone towards the completion of the exercise.

### 3.2 Make commits that satisfy the issues

The open issues is like a ToDo list that tells you what needs to be done. Usually Issues grow with feedback from collaborators or your own insights. This can save you a lot of emails that are out of context. Now, implement the changes suggested in the issues.

:arrow_right: Make the required commits to solve all the issues.

:bulb: If you include the phrase "Closes #123" as part of your commit message, Github will automatically close Issue #123 and will indicate which commit closed it. You can use any of these keywords close, closes, closed, fixes, fixed followed by the commit #id number.

Your corrected file should look like this:

```
Target Name      Instrument      Frequency (GHz)    Sensitivity (μJy)
NGC 4321         VLA             1.4                60
M87              ALMA            230                2.5
NGC 6946         MeerKAT         1.4                15
M51              VLA             3.0                5
Andromeda        GMRT            0.325              100
NGC 253          ALMA            115                8
```


# <a name='exercise3-branches-pr'></a>Exercise 3 - How to manage branches and Pull Requests

:pill: **Aim of this exercise**
Branches allow you to develop features, fix bugs, or experiment with new ideas in a contained area of your repository isolated from the original repository.
*The idea is to create one branch, add content and update the original repository with the changes.*

<HR>

In this exercise, one branch will be created. Let's say that this new branch will include new features we want to implement or improve to the existing repository. Since this work will take a long time, we want to keep it separated from the main repository until we finish the work in progress and the changes are matured.

### 3.1 Create a new file named `report.tex`

Go to the repo home page, select `Add file` and create a new file named `report.tex` and fill it with this content:

```
\documentclass{article}
\title{Galaxy Properties Report}
\author{}
\date{}

\begin{document}

\maketitle

\section{Introduction}
This report summarizes key properties of selected galaxies.

\section{Galaxy Data}
The galaxy \textbf{<Galaxy Name>} is classified as a \textit{<Type>} galaxy. 
It is located at a distance of <Distance> Mpc, with a redshift of <Redshift>.

\end{document}
```
:arrow_right: You have work to do! First, create a new issue and assign yourself to it. Mention that you need to fill relevant information for a publication you are working on.


### 3.2 Create a new branch `update-galaxy-data`.

In the repository main page, click the buttom on the top left labelled as `main`. In the search box write **`update-galaxy-data`** and then press "Create branch update-galaxy-data from main".

![exercise example 3](./media/exercise3.1.png)

You will see that when you select this icon, all the available branches will appear and you can switch between them to make changes in each one.

![exercise example 3](./media/exercise3.3.png)

:bulb: Note that the repository contents and files may be different for each branch.

### 3.3 Modify the file `report.tex` inside the branch `update-galaxy-data`

Now we are going to switch to the **`update-galaxy-data`** branch and to modify the `report.tex` file. Replace placeholders (\<Galaxy Name\>, \<Type\>, \<Distance\>, \<Redshift\>) with real data for a galaxy of your choice (e.g., "NGC 4321," "Spiral," "16.8," "0.007").

:arrow_right: Create a commit to modify the file. Write an informative commit message.

### 3.4 Prepare the pull request

Once this is done, we are going to merge the changes from the **`update-galaxy-data`** branch with the **`main`** branch.

You will notice that in the main repository there will be a warning indicating that a branch has been modified and suggesting you to "Compare and pull request". This will take you directly to initiate the pull request. When there are many active branches, it is safer to navigate to the relevant branch. To do this, click on `view branches` and then on `view all branches`:

![exercise example 3](./media/exercise3.4.png)

From here we can merge the changes made in the development branch with the main branch and original repository. Click on the `New pull request` button to do this.

A Pull Request has a title, which should be clear and informative, and a description that explains the nature of the changes. This is important when collaborating with other people (remember, consider the future you as a collaborator).

:arrow_right: Create the Pull Request

:bulb: Note the message next to the green buttom Open at the top: "\<your user\> wants to merge 1 commit into main from update-galaxy-data". This is important to keep track of the origin and destination of the PR.

:arrow_right: Navigate to the "Pull Requests" tab and confirm that your PR is there and it is Open

### 3.4 Merge pull request

Inside the Pull Request, Github will verify that there are no conflicts (i.e., that nobody else modified the same part of the file(s) you modified inside the branch). Then you should see the message "This branch has no conflicts with the base branch.  Merging can be performed automatically". 

:arrow_right: Press merge pull request

:arrow_right: Press Confirm merge

Now your changes leave in the main repository, indicating that they are mature and ready to be seen by everyone. 

:bulb: since all commits are not part of the main repository, you can delete the branch if you will not need it anymore.

:arrow_right: Navigate to the "Pull Requests" tab and confirm that your PR is now Closed.


# <a name='exercise4-collaborate-fork'></a>Exercise 4 - Collaborate in a repo. Fork a repository

:pill: **Aim of this exercise**
In this exercise we are going to use an existing repository to :fork_and_knife: *Fork* and interact with it, and finally propose some changes to be merged with the original existing repository by using a *Pull Request*. 
*The idea is to collaborate with an existing repository to propose some changes to the content.*

<HR>

To do this, we first go to this repository by clicking this link: 

https://github.com/manuparra/mparra-csic-github

Then, from the top right menu click the :fork_and_knife: *Fork* button and you will see a screen to select which organisation (of which you are a member) will do this operation, select one of them and in a few moments the repository will be a fork of the original one. If you are not a member of an organisation, it will directly :fork_and_knife: *Fork* the repository.

After that, you should see something like this, where the name of the repository is indicated and below it the original repository of the :fork_and_knife: *Fork*:

 ![exercise example 1](./media/exercise2.1.png)

In this moment you are working with a :fork_and_knife: *Forked* copy of the original repository.
	
Now you have to make the following change:

- Use the `Add` option to include a `FOLDER` with your name and inside that folder a `README.md` file with the following text:


:warning: In order to create this `FOLDER`, use the first letter of your first name and your first surname. 
> :radioactive: :bulb: For example: If your name is `Manuel Parra`, your FOLDER and FILE path will be:
> `mparra/README.md`
> :warning: Use a path to create the file.

Paste the following text to the 

```
# Course of Reproduciblity @CSIC

In this course I will learn:
- Control version platforms like GitHub, containers and more!

```

:arrow_right: `Commit` the change and add a short description of this change with the following text: `Updated folder and README.md`

Now it is time to contribute the changes made by making a *Pull Request*, i.e. requesting the original repository that we *"would like"* to include these changes in the original repository. 

To do this go to the main repository screen and select the following option:

 ![exercise example 1](./media/exercise2.2.png)


Doing this, it checks that there are no conflicts and you can propose the change by including a comment about the changes you want to push to the original repository. 

![exercise example 1](./media/exercise2.3.png)

Include a title and a short description and then click `Create pull request`:

![exercise example 1](./media/exercise2.4.png)

Once this is done, you will have to wait for the original repository owner to review the request and accept it. When this happens you will be notified in a short time :smile: .


###  2.4. <a name='Exercise4-Collaboratingwithotherrepositoriesandusers-Homework'></a>Exercise 4 - Collaborating with other repositories and users - Homework

:pill: **Aim of this exercise**
The aim of this exercise is for the student to be able to interact with the repository by collaborating with other users through the management of `Issues` and working with copies of repositories among the students.

<HR>

For this exercise you need to use the list of users and repositories listed in [this link](https://hackmd.io/s/B1zp3lJm5). On this page, go to exercise 4 and find your name and the tasks you have to perform with each of these repositories.

The tasks to perform for this exercise are as follows:

- :one: Find your name in the list on this [link](https://hackmd.io/s/B1zp3lJm5).
- :two: Two tasks will appear, 
  - a) Make a fork of the repository listed below your name and then, 
  - b) Create an Issue on the second repository.


**For the first :one: repository** you have to make a fork of this repository and add a **directory** with your `namesurname` and a **file** inside named `plot.py` containing the following:

```
import matplotlib.pyplot as plt
plt.plot([1, 2, 3, 4])
plt.ylabel('some numbers')
plt.show()	
```
Once this is done you must `Create a Pull Request` with this change to the original repository.
	
**For the second :two: repository** you have to create at least one issue to the repository, to make one of the following changes, which the **repository owner** must do:
- a) Request to include a file with a science image.
- b) Request to include a data file.
- c) Request to add more information to README.md related to the aims.
- d) Report a typo for correction 

:bulb: *Use the @ to type the name of the repository owner for direct notification. For example: @manuparra*.
