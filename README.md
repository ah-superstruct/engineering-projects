# Engineering Projects Repository

This repository functions as a main holding space for all projects's documentation in their creation and planning stages.

---

## Workflow

### **Step 1**

Product creates and issue in this repository. This issue should contain all necessary information needed to allow Engineering to estimate a deploy date and total project hours.

### **Step 2**

Engineers are assigned and engineer creates PR.

```Note: ***This PR will not be closed until the issue it addresses is closed.***```

#### PR Structure

When first created, the PR should:

- have its branch named after its project in `camelCase`
- have its name be the same name as the issue it addresses.
  - ex. `00001 ProjectName`
  - Note that `00001 === Issue Number` <-(Padded to 5 integers) & `ProjectName === Issue Name`
- have 'closes: $issue' in its desccription.
  - ex. closes: #1

### **Step 3**

Assigned Engineer will proceed to document their plan to deploy the project in a series of commits.

### **Commit 1:** Create Planning Document Markdown Sheet

- Link to main issue in Engineering Projects Repository
  - ex. [Example Project](https://github.com/ah-superstruct/engineering-projects/issues/1)

### **Commit ```2 + n```:** Generate [Planning Outline](./planningOutline.md)

- May take as many commits as needed to complete.

### **Step 4**

The PR description is updated with estimations using the information gained from completing the [planning outline](./planningOutline.md).

***Important:***

Should the main project exceed ```60``` hours, sub-projects and their corresponding issues will be [created](README.md#step-7) and referenced in description as they are created and estimated.

Estimations for the project and sub-projects should bbe formatted as such:

> ``` Javascript
> Project <STRING>: 'Project Name'
> ```

> ``` Javascript
> Hour Estimation <INT>: 0 - 60 'Number Of Hours Estimated To Deploy'
> ```

> ``` Javascript
> Optimal RTD <DATE>: Optimal Date To Deploy => MM/DD/YYYY
> ```

> ``` Javascript
> Estimated RTD <DATE>: Date Ready To Deploy => MM/DD/YYYY
> ```

> ``` Javascript
> Project Planning Outline <URL>: [Link To Project Planning Markdown File On PR Branch]()
> ```

### **Step 5**

The assigned engineer then reaches out to the Engineering Manager and asks for the green-light to proceed.

### **Step 6**

Upon getting the green-light, the engineer posts their estimations in #engineering-projects

### **Step 7**

Using the [planning outline](./planningOutline.md), the assigned engineer creates the necessary issues in the respective repositories as necessitated by the project's scope. These issues will be the ones that the assigned engineer will be working on closing when working on the project itself. 

> As these issues are created, they should be referenced and linked in the PR's description.

### **Step 8**

Engineers continue work on the Project until all tickets and related issues are completed. Once everything is deployed, the main issue that was opened in Engineering Projects Repository will be closed by using the original PR made to hold the planning outline and estimation information.
