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
- [Exercise 4 - Collaborate in a repository. Fork a repository](#exercise4-collaborate-fork)

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


Now, explore your repository. You will have only two files: LICENSE and README.md. Let's add some information about your repository by modyfing the `README.md` file. Click on the file and then on the edit button on the right.

![image](https://github.com/user-attachments/assets/8675eccd-0d48-4d83-a274-56e1c085daa4)

![image](https://github.com/user-attachments/assets/eef45687-b0bc-4991-893c-d521211f7eba)

Use the following text to update the `README.md` file.

```
## SO-IAA training course: Introduction to Github

This is the working repository for the course exercises.
This repository will be used to practise commits, issues, branching and pull requests. 

# Session 2

## Creating a new repository and adding content

- [ ] Created repository
- [ ] Updated content

```
:arrow_right: Commit the change

### 1.2 Populate the repository with a data table

Once the README is ready, add the following data file named `power.csv`. Press "Add file" and "+ Create new file". 

![image](https://github.com/user-attachments/assets/59ac9aec-3eb0-4123-9d4d-84eff1c51a93)

Copy and paste the following content to the new file:

```
date,max,avg,min
2021-10-05 15:00,5285.0,4126.0,3968.0
2021-10-05 15:15,5292.0,4125.0,3953.0
2021-10-05 15:30,5296.0,4125.0,3950.0
```

:arrow_right: Commit the change

### 1.3 Edit an existing file

Once this change is made, navigate to the file and Edit it pressing on this button:

![image](https://github.com/user-attachments/assets/f8fa8fc3-b2c5-4014-a12f-b72e49bd77d5)

Add a couple more lines of data to the `power.csv` file

```
2021-10-05 15:45,5287.0,4123.0,3952.0
2021-10-05 16:00,5234.0,4122.0,3965.0
```

:bulb: Press "Preview" to see a direct before/after comparison. Green are new content, red means removed content.

:arrow_right: Commit the change

:checkered_flag: :checkered_flag: After these steps, you can check the version history. 

![image](https://github.com/user-attachments/assets/35c05caa-9b97-4e18-9ff9-533bc4b1d3ef)

:arrow_right: Visit the commit history and explore the file at different versions (different commits). Also, click on the commit id to see the changes.

![image](https://github.com/user-attachments/assets/8832dcab-18df-48ae-b2a5-712981871364)


👩‍🎓 For advanced students: find the repo of your companion, and add issues asking them to modify their repo. Give clear instructions. Your companion may want to discuss how the issue should be implemented.

# <a name='exercise2-issues'></a>Exercise 2 - Plan and manage your work: Issues

:pill: **Aim of this exercise**
Issues allow you to track ideas (bugs that need fixing, new implementation ideas, suggested changes, ToDos), allowing interaction and discussions in an organized way. Usually a commit serves to solve a particular issue. *The idea is to plan a series of changes to a daba table by creating Issues, and then commit the changes that solve them*

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

:arrow_right: Create the following issues and add these descriptions:

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

:bulb: If you include the phrase "Closes #123" as part of your commit message, Github will automatically close Issue #123 and will keep track of which commit closed it. You can use any of these keywords "close", "closes", "closed", "fixes", fixed followed by the commit #id number.

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
:arrow_right: Visit the commit history and explore the file at different versions (different commits).

![image](https://github.com/user-attachments/assets/8832dcab-18df-48ae-b2a5-712981871364)


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

In the repository main page, click the button on the top left labelled as `main`. In the search box write **`update-galaxy-data`** and then press "Create branch update-galaxy-data from main".

![exercise example 3](./media/exercise3.1.png)

You will see that when you select this icon, all the available branches will appear and you can switch between them to make changes in each one.

![exercise example 3](./media/exercise3.3.png)

:bulb: Note that the repository contents and files may be different for each branch.

### 3.3 Modify the file `report.tex` inside the branch `update-galaxy-data`

Now we are going to switch to the **`update-galaxy-data`** branch and to modify the `report.tex` file. Replace placeholders (\<Galaxy Name\>, \<Type\>, \<Distance\>, \<Redshift\>) with real data for a galaxy of your choice (e.g., "NGC 4321," "Spiral," "16.8," "0.007").

:arrow_right: Create a commit to modify the file. Write an informative commit message. Note that the commit window will inform you about the branch that will contain this commit.

### 3.4 Prepare the pull request (PR)

Once this is done, we are going to merge the changes from the **`update-galaxy-data`** branch with the **`main`** branch.

You will notice that in the main repository there will be a warning indicating that a branch has been modified and suggesting you to "Compare and pull request". This will take you directly to initiate the pull request. When there are many active branches, it is safer to navigate to the relevant branch. To do this, click on `view branches` and then on `view all branches`:

![exercise example 3](./media/exercise3.4.png)

After selecting the relevant branch, we can merge the changes made with the main branch. Click on the `New pull request` button to do this.

A Pull Request (PR) has a title, which should be clear and informative, and a description that explains the nature of the changes. This is important when collaborating with other people (remember, consider the future you as a collaborator). A PR may consist of multiple commits.

:arrow_right: Create the Pull Request

:bulb: Note the informative message on the top, where you can see which branch do you propose to merge (e.g., new-branch) and where it will be merged (a.g., main). You will see something similar to: "\<your user\> wants to merge 1 commit into main from update-galaxy-data". This is important to keep track of the origin and destination of the PR.

![image](https://github.com/user-attachments/assets/00f30583-70b9-4f7b-bb7d-55f2b76228ea)

:arrow_right: Navigate to the "Pull Requests" tab and confirm that your PR is there and it is Open.

### 3.4 Merge pull request

Inside the new *Pull Request*, Github will verify that there are no conflicts (i.e., that nobody else modified the same part of the file(s) you modified inside the branch). Then you should see the message "This branch has no conflicts with the base branch.  Merging can be performed automatically". 

:arrow_right: Press merge pull request

:arrow_right: Press Confirm merge

Now your changes leave in the main repository, indicating that they are mature and ready to be seen by everyone. 

:bulb: Since all commits are now part of the main repository, you can delete the branch if you want, since you will not need it anymore.

:arrow_right: Navigate to the "Pull Requests" tab and confirm that your PR is now Closed.


# <a name='exercise4-collaborate-fork'></a>Exercise 4 - Collaborate in a repository. Fork a repository

:pill: **Aim of this exercise**
In this exercise we are going to use an existing repository to :fork_and_knife: *Fork* and interact with it, and finally propose some changes to be merged with the original existing repository by using a *Pull Request*. 
*The idea is to collaborate with an existing repository to propose some changes to the content.*

<HR>

We are going to contribute to the repository of someone external, so we don't have access to modify it. In particular, we will use this example repository:

[Galaxy Database Project](https://github.com/iaa-so-training/github2024_session2/tree/main)

This repository needs a lot of improvements, which are described in a series of already existing Issues: [Issuse of Galaxy Database Project](https://github.com/iaa-so-training/github2024_session2/issues).

:arrow_right: Go to the Issues list and identify one that would like to solve and write a new comment saying that you want to work on this problem.

:bulb: since you are not a member of the repository, you cannot be assigned an issues. However, once you commented, Github will allow the owner to assign the issue to you. 

Note that more than one person may be interacting with the issue at the same time, so the owner will decide one or more people will be assigned. This assignation is just a formatlity that helps organizing big repositories, but you can still open a Pull Request at any time.

Since you don't have editing permissions in the original repo to be able to contribute, we will fork (*duplicate*) the repository in our own account, and then we will create a pull request towards the original repository.

### 4.1 Fork an external repository to your account and create a new branch

Navigate to the [Galaxy Database Project](https://github.com/iaa-so-training/github2024_session2/tree/main) repository. From the top right menu click the :fork_and_knife: *Fork* button and you will see a screen to select the owner (usually you, but can also be an organisation) of the forked repository. In a few moments the repository will be a fork of the original one. If you are not a member of an organisation, it will directly :fork_and_knife: *Fork* the repository under your user name.

After that, you should see something like this, where the name of the repository is indicated and below it the original repository of the :fork_and_knife: *Fork*:

 ![exercise example 1](./media/exercise2.1.png)

In this moment you are working with a :fork_and_knife: *Forked* copy of the original repository.

:arrow_right: Create a new branch in the forked repository.

:bulb: If in doubt, see Exercise 3.2 above. Or navigate to "See all branches" and click "New Branch".

### 4.2 Edit your fork to solve the issues from the original repository

Find the relevant issues in the main repository. Edit the relevant files and modify them following the specific instructions in the repository. 

:arrow_right: make one commit that specifically solves one issue. Write a clear and specific commit message.

### 4.3 Propose to merge your changes with the original repository

Now it is time to contribute the changes made by making a *Pull Request*, i.e. requesting the original repository that we *"would like"* to include these changes in the original repository. 

To do this go to the main repository screen and select the following option:

 ![exercise example 1](./media/exercise2.2.png)

Doing this, it checks that there are no conflicts and you can propose the change by including a comment about the changes you want to push to the original repository.

![exercise example 1](./media/exercise2.3.png)

Include a title and a short description and then click `Create pull request`

:bulb: You can add "Solves #X" with X being the number indentifier of the issue in the original repository (only if you are a member of the repository, otherwise only the contributors can close an issue).

![exercise example 1](./media/exercise2.4.png)

Once this is done, you will have to wait for the original repository owner to review the request and accept it. When this happens you will be notified in a short time :smile: .

:arrow_right: Go to the original repository and explore both the Issues and the Pull Request tabs. Check the status of your PR.

:bulb: Navigate to the "Insights" tab and open "Networks". There you will see the full story of the commits and their flow from different forks.

As you can image, the full flow of a large package can be very complicated and intricated. This methodology ensures that contributors can collaborate effienctly. 

### 4.4 Contribute further to the repository

If you have time, explore the remaining Issues. Assign one to you to let the other contributors know that you want to work on it. You may want to write a new comment to indicate so. Repeat the cycle: create a branch (this is optional, since the changes are simple) in your forked repo, commit changes and open a Pull request.

Feel free to suggest additional changes to any of the existing files, the Readme, etc.

:bulb: You will need to synchronize your forked repo frequently, since changes may had happened in the original repo (*upstream*).


# End of the course

Congratulations for finishing the exercises. Now you have a final task to confirm that you completed the course:

:arrow_right: In the course repository [introduction_github2024](https://github.com/iaa-so-training/introduction_github2024/tree/main), edit the attendants file to add your name. You will receive an attendance certificate only if your name is there.

:bulb: If you find some of the material of the course can be improved, please open an Issue and, if possible, make a PR with your contribution to improve the contents.
