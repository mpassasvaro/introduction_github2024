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
* 2. [Exercises](#Exercises)
	* 2.1. [Exercise 1 - Create an initial repository. Issues, commits and history](#Exercise1-Createaninitialrepositoryforthissession)
	* 2.2. [Exercise 2 - How to manage branches and Pull Requests](#Exercise2-Branches)
	* 2.3. [Exercise 3 - Collaborate in a repo. Fork a repository](#Exercise3-CollaborateFork)

<!-- vscode-markdown-toc-config
	numbering=true
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->

<HR>


##  2. <a name='Exercises'></a>Exercises

###  2.1. <a name='Exercise1-Createaninitialrepositoryforthissession'></a>Exercise 1 - Create an initial repository for this session

:pill: **Aim of this exercise**
In this exercise a new repository will be created and some modifications and data files will be added. Finally, the history of changes made will be reviewed.

<HR>

For this training exercise it will be necessary to create a new repository with the following initial details: 

- Repository name: ``so-github-course``.
- Repository description: ``Repository for the exercise 1``.
- Repository scope: ``Public``.
- Licence: For example select the ``MIT licence``.
- Add a default ``README.md``.

In the following image you can see the options to select for the creation of the repository:

 ![exercise example 1](./media/exercise1.1.png)

Add some information to your repository by modyfing the `README.md` file. Use the following text to update the `README.md` file.

```
# SO Github course: Introduction to Github

This is the working repository for the course exercise 1. 

# Session 1

## During this exercise I will conduct the follow tasks:

- [ ] Created repository
- [ ] Update README file

```
:arrow_right: Commit the change

After including this change, create a folder with the name `data` and add a file named `power.csv`, copying and pasting the following content:

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


###  2.2. <a name='#Exercise2-Issues'></a>Exercise 2 -  Managing issues

We will manage a series of tasks that need to be done. Issues can be thought as a ToDo list, that can be created by you or by your collaborators. It allows you to have discussions by adding comments, which facilitates communication with collaborators (or with your future self).

Create three issues in your repository. Assign them to you. You may want to create a milestone to indicate that these issues are needed to complete Exercise 1.

**Issue 1: Create the file power.csv in the repository**

Create a file called `my_collaborators.txt` and fill it with:
```
Name        Age        City
Alice       25         New York
Bob         30         
Eve                    Los Angeles
```

**Issue 2: Missing data for Bob's city**

Bob's City field is empty. Update it with "San Francisco."

**Issue 3: Missing data for Eve's age**

Eve's Age field is missing. Update it with "28."

**Issue 4: Align table formatting**

The table has inconsistent spacing. Reformat it for proper alignment.


:arrow_right: Commit the changes needed to complete the three issues and mark them as *Closed*.

:checkered_flag: :checkered_flag: After these steps, you can check the version history. 


###  2.3. <a name='#Exercise3-CollaborateFork'></a>Exercise 3 - Managing branches

:pill: **Aim of this exercise**
Branches allow you to develop features, fix bugs, or experiment with new ideas in a contained area of your repository isolated from the original repository.
*The idea is to create one branch, add content and update the original repository with the changes.*

<HR>

In this exercise, one branch will be created. Let's say that this new branch will include new features we want to implement or improve to the existing repository.

For this exercise you have to go to the repository *"Forked"* in the previous exercise. 

Once in the *Forked* repository we have to add a new branch.

To do this, create a new branch from the next option on the main screen of your repository and name it **"\<namesurname\>-development"**. 

![exercise example 3](./media/exercise3.1.png)


You will see that when you select this icon, all the available branches will appear and you can switch between them to make changes in each one.

![exercise example 3](./media/exercise3.3.png)

Now we are going to switch to the **"\<namesurname\>-development"** branch and to modify the `README.md` file, adding the following lines to the end of it:

```
# Session 1: Exercises 3 from <namesurname>
- Created a new branch for development.
```

:warning: In order to add this text, within the `<namesurname>` string, use the first letter of your first name and your first surname. 
> :radioactive: :bulb: For example: If your name is `Manuel Parra`, your text will be:
> ```
># Session 1: Exercises 3 from mparra
>Created a new branch for development.

Once this is done, we are going to merge the changes from the **"\<namesurname\>-development"** branch with the main branch. To do this, click on `view branches` and then on `view all branches`:

![exercise example 3](./media/exercise3.4.png)

From here we can merge the changes made in the development branch with the main branch and original repository. Click on the `New pull request` button to do this. 

🏁 🏁 Soon your changes will be accepted by the repository owner.



###  2.4. <a name='#Exercise2-Branches'></a>Exercise 2 -  Managing forks to collaborate

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


- d) Report a typo for correction 

:bulb: *Use the @ to type the name of the repository owner for direct notification. For example: @manuparra*.
