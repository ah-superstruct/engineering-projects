# Engineering Projects Repository

This repository functions as a main holding space for all projects in their creation and planning stages. 

### Repository Structure

This repositories structure is simple. We have a main folder that holds all planning markdown files. New projects are created in the form of new issues by Product. 

### Workflow

1. Product creates and issue in this repository. This issue should contain all necessary information needed to allow Engineering to estimate a deploy date and total project hours. 
	a. Assigned engineer opens a PR that closes Product's issue.
	b. Assigned engineer then creates a markdown file labeled the following way: 

``` JavaScript
00001 ProjectName

Note: 
00001 === Issue Number ('Padded to 5 integers')
ProjectName === Issue Name
```

2. Within this markdown sheet the assigned engineer will add the following:
- Link to main issue in Engineering Projects Repository
- [Planning outline](README.md#planning-outline)

3. After the information is gathered for the [Planning outline](README.md#planning-outline), a commit should be pushed into the PR with the information formatted as so: 

``` Javascript
Project <STRING>: Project Name
Hour Estimation <INT>: Number Of Hours Estimated To Deploy
Optimal RTD <DATE>: Optimal Date To Deploy => MM/DD/YYYY
Estimated RTD <DATE>: Date Ready To Deploy => MM/DD/YYYY
Project Planning Outline <URL>: Link To Project Planning File
```

4. The assigned engineer then reaches out to the Engineering Manager and asks for a greenlight to proceed.

5. Using the planning outline, the assigned engineer creates the neccessary issues in the respective repositories as necessitated by the project's scope. These issues will be the ones that the assigned engineer will be referenceing when working on the project itself. 

6. Push another commit to add in links to the issues created in the production repositories.

7. Continue working on the Project until all tickets and related issues are completed. Once this is done, the main issue that was opened in Engineering Projects Repository can be closed with the original PR made to hold the planning outline and estimation information. 

## Planning Outline

In order to facilitate proper forethought and planning in a project, a planning outline should contain the following, at a minimum:

#### What is the objective?
- Why? 
- Who is asking for this?
- What happens if we don't do this? 

#### What is the current state of the system this project will affect? 
- How does it work?
- What is the system flow step by step?

#### What are different ways to achieve the objective? 
- Option 1
	- What changes need to me made to: 
		- Front End?
		- Back End?
		- User documentation?
		- Business itself?
- What are the advantages?
	- How much code needs to be changed? 
	- How quickly can this be done? 
	- How many people need to be involved? 
	- What are the operational changes? (database, hosting, etc)
- What are the risks? 
	- Can this be reversed? 
	- What kind of maintenance is involved? 
	- Would a new developer or user be able to understand this? 
	- Will this cause technical debt?
- Option 2
- Option 3

#### What is the recommendation moving forward? 
- Which option is best? 
- Why? 
	- Which advantages are most important?
	- Which drawbacks are acceptable?
- What are the next steps?
	- What tickets need to be created? 
	- How many hours will each ticket take?
	- What is the estimated date to deployment of the project?

## Project Division
