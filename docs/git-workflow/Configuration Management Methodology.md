<p align="center">
  <img src="../../images/logo/Logo%20-%20Marmara%20Üniversitesi%20with%20name.png">
</p>

<p align="center"><u><b><span style="font-size:25px">Configuration Management Methodology (Git-Workflow)</span></b></u></p>
<p align="center"><b><span style="font-size:20px">Artificial Intelligence Used for Disease Prediction</span></b></p>

<br></br>

<table align="center" style="border: 1px solid black; width: 90%; padding: 10px;">
<tr>
    <td colspan="2">
      <table align="center">
        <tr>
          <th style="text-align: center;">Repository</th>
        </tr>
        <tr>
          <td style="text-align: center;"><b><a href="https://github.com/mtlgkbb20/ReportAutomation">https://github.com/mtlgkbb20/ReportAutomation</a></b></td>
        </tr>
      </table>
    </td>
  </tr>
  <tr>
    <td>
      <table style="margin-right: 30px;">
        <tr>
          <td>
            <p align="center">
              <b><span style="font-size:20px">Project members</span></b>
            </p>
            <table style="border-collapse: collapse;">
              <tr>
                <th style="text-align: left; padding-left: 20px;">Pablo Buza Mira</th>
                <td style="padding-left: 20px;">199524008</td>
              </tr>
              <tr>
                <th style="text-align: left; padding-left: 20px;">Aleyna Çakır</th>
                <td style="padding-left: 20px;">150820023</td>
              </tr>
              <tr>
                <th style="text-align: left; padding-left: 20px;">Hümeyra Eda Devrim</th>
                <td style="padding-left: 20px;">150820071</td>
              </tr>
                <tr>
                <th style="text-align: left; padding-left: 20px;">Leen I. A. Shaqalaih</th>
                <td style="padding-left: 20px;">150121921</td>
              </tr>
              <tr>
                <th style="text-align: left; padding-left: 20px;">Mustafa Tolga Akbaba</th>
                <td style="padding-left: 20px;">150120001</td>
              </tr>
                <tr>
                <th style="text-align: left; padding-left: 20px;">Selin Aydın</th>
                <td style="padding-left: 20px;">150120061</td>
              </tr>
              <tr>
                <th style="text-align: left; padding-left: 20px;">Zehra Savaş</th>
                <td style="padding-left: 20px;">150820062</td>
              </tr>
            </table>
          </td>
        </tr>
      </table>
    </td>
    <td>
      <table>
        <tr>
          <td>
            <p align="center">
              <b><span style="font-size:20px">Recipient Information</span></b>
            </p>
            <table style="border-collapse: collapse;">
              <tr>
                <th style="text-align: left;">Professor</th>
                <td style="padding-left: 20px;">Şakir Bingöl</td>
              </tr>
              <tr>
                <th style="text-align: left;">Course</th>
                <td style="padding-left: 20px;">EE4056 - Introduction to Information Systems Management</td>
              </tr>
              <tr>
                <th style="text-align: left;">Classroom</th>
                <td style="padding-left: 20px;">RTEM4.126</td>
              </tr>
              <tr>
                <th style="text-align: left;">University and Faculty</th>
                <td style="padding-left: 20px;">Marmara University, Faculty of Engineering</td>
              </tr>
            </table>
          </td>
        </tr>
      </table>
    </td>
  </tr>
</table>

<br></br>

---

# Table of Contents

- [Intent](#intent)
- [Revision Table](#revision-table)
- [Introduction](#introduction)
- [A. Coding Standards](#a-coding-standards)
  - [A.1. Naming Conventions](#a1-naming-conventions)
  - [A.2. Indentation and Code Formatting](#a2-indentation-and-code-formatting)
  - [A.3. Comments and Documentation](#a3-comments-and-documentation)
  - [A.4. Line Length Convention](#a4-line-length-convention)
  - [A.5. Error and Exception Handling](#a5-error-and-exception-handling)
- [B. Confirming Message Policies](#b-confirming-message-policies)
  - [B.1. Commit Messages](#b1-commit-messages)
    - [B.1.1. General Rules](#b11-general-rules)
    - [B.1.2. Specific Rules](#b12-specific-rules)
- [C. Branching Structure](#c-branching-structure)
- [D. Branching Strategy Based on GitFlow Including Peer Reviews](#d-branching-strategy-based-on-gitflow-including-peer-reviews)
  - [D.1. How to Develop Feature Branches](#d1-how-to-develop-feature-branches)
  - [D.2. How to Prepare Releases](#d2-how-to-prepare-releases)
  - [D.3. How to Fix Production Bugs](#d3-how-to-fix-production-bugs)
- [E. Versioning Policies](#e-versioning-policies)
- [F. Definition of Done](#f-definition-of-done)
- [G. Document Management in the Repository](#g-document-management-in-the-repository)
- [Conclusion](#conclusion)
- [Bibliography](#bibliography)

<br></br>

# Intent

The purpose of this report is to describe the agreed-upon approach for the project configuration management methodology that the team will follow. This methodology is generated by consensus among the team members and serves to better organize the work.

<br></br>

# Revision Table

<table border="1">
  <tr>
    <th>Revision Number</th>
    <th>Revision Date</th>
    <th>Description of the Revision</th>
    <th>Performed by</th>
  </tr>
  <tr>
    <td>1</td>
    <td>25/03/2025</td>
    <td>The overall document structure and information was planned and implemented.</td>
    <td>Pablo Buza Mira</td>
  </tr>
</table>

<br></br>

# Introduction

This document describes the configuration management methodology agreed upon for application in the project by the team. To do so, it will mention trivial aspects such as the branching strategy based on GitFlow, the naming pattern to be followed when writing commit messages, or the project versioning rule.

<br></br>

# A. Coding Standards

In this section, the programming standards that will be followed in the project are detailed, with the objective of ensuring code and documentation consistency and quality, as well as promoting best practices in the development process.

## A.1. Naming Conventions

For handling all the project documentation and/or code, the following standards have been followed:

- For variable, method, and parameter names, use the camelCase convention, where the first letter of each word except the first is written in uppercase. For example: userName, totalNumber.
- For entity names, use PascalCase, where the first letter of every word is capitalized. These names should not be long (they should not exceed 5 words). For example, you cannot use: MarmaraUniversityPersonalIdentificationNumber, instead you should use: PersonalID.
- Folders within `src` are written in all lowercase.
- Folders within `frontend` are written in camelCase.

## A.2. Indentation and Code Formatting

Tabulations equivalent to 8 spaces (default tabulation) will be used. Code inside the braces corresponding to conditional statements and loops (`for`, `if`, `while`, `switch`), as well as inside class and method declarations, will be indented.

The aim is to maintain consistency in spacing and indentation, also improving the code’s readability and visualization.

## A.3. Comments and Documentation

Document the code using clear and concise comments to explain the purpose of functions and complex algorithms without overusing them.

There is no maximum word count per comment, although it is recommended to explain clearly, concisely, and briefly every comment that is added.

Redundant comments, either due to the code itself or project documentation or already included comments, will not be employed.

## A.4. Line Length Convention

Lines of code longer than 120 characters will be avoided.  
If a line of code is too long, it will continue on the next line with an indentation tab for the subsequent lines.

## A.5. Error and Exception Handling

Implement a consistent strategy to handle errors and exceptions in the code, using try-catch, code debugging processes (both on the client and server side), or by seeking help from the rest of the project team.

<br></br>

# B. Confirming Message Policies

The following commit policy aims to establish guidelines and best practices for managing commits in the GitHub repository. This will ensure consistency, effective collaboration, and traceability of the change history in the project.

## B.1. Commit Messages

To make a commit, the following rules must be followed:

### B.1.1. General Rules

When writing commits, we will follow the best practices recommended in the course so that the commits are descriptive, atomic, cohesive, coherent, and represent a logical increment. Following this line, it will be necessary to:

- Separate the title and the body of the message with a blank line.
- (Optional) Separate the body of the message and the footer with a blank line.
- Limit the title to below 50 characters, not including the 'type' in this maximum character count.
- Do not use a period at the end of the title.
- Use the imperative mood in the title.
- The lines in the body should be limited to 72 characters.
- Use the body of the message to explain what and why versus how.

### B.1.2. Specific Rules

Every commit must follow the following structure:

1. **Title:**  
   The title will have the following structure: `<type>: <description>`, where:

- `type` can be:

  - `Feat` for new functionalities or features that imply minor changes.
  - `Fix` for fixing or correcting errors in the code or documentation.
  - `Docs` for adding or updating documents.
  - `Chore` for handling administrative or maintenance tasks, such as updating dependencies or refactoring code.
  - `Test` for tasks related to testing.

- `type` can include a `!` after the type to indicate a 'BREAKING CHANGE'.

- `description` will be a brief description of the task performed.

2. **Message Body:**  
   A short explanatory paragraph that complies with the general rules mentioned above.

3. **Footer:**  
   The footer is optional, although highly recommended.  
   The footer will include:

- `BREAKING CHANGE`, if applicable, provided that `!` was not included after the `type`.
- `Refs #issue`, to indicate which issue the commit is related to.

<br></br>

# C. Branching Structure

The repository will contain the following branches:

- **`main` or `master`**: the primary branch that is in a production state, ready to produce a new release.

- **`develop`**: a branch that points to the latest development version for the next release. It will include the latest changes implemented for the upcoming delivery, created from the `main` or `master` branch and, in general, will contain complete functionalities without major errors.

- **Feature Branches**: branches used to develop new functionalities that will be added in the next release. There will be a new branch for each functionality created from `develop`; when completed, the changes will be merged back into it.

- **Release Branches**: branches used to prepare a new version of the application. In these branches, small changes (such as fixing minor bugs, last-minute changes, etc.) will be made. They are generated from `develop` and, on them, the final necessary changes will be made before putting the project into production. The changes will be merged into both `develop` and `main` (or `master`).

- **Hotfix Branch**: this branch will be used to fix critical bugs in the production version. It is created from the `main` or `master` branch.

<br></br>

# D. Branching Strategy Based on GitFlow Including Peer Reviews

In our project, we have chosen to implement a branching strategy based on GitFlow, which is a very popular branching model that defines a clear structure for collaborative software development, based on the existence of different types of branches to manage various stages of the software lifecycle: `main` or `master`, `develop`, `feature`, `release`, and `hotfix`. _NOTE: If a feature involves adding a document or other multimedia content, you may use "doc" or "multimedia" instead of "feature"._

This strategy provides a structured framework to manage the workflow in a Git repository, enabling efficient and organized collaborative development. In the following subsections, we will detail how we will use GitFlow, including the creation of feature branches, release preparation, and production bug fixes, all with peer reviews to ensure code quality.

It is important to remember that peer review is fundamental to enhance the shared knowledge that team members have about the project, promote the use of coding standards, improve code quality, and reduce the "bus factor" (i.e., the risk the project faces if a key person stops working on it).

## D.1. How to Develop Feature Branches

To develop new features in our project, we will follow the procedure below:

1. **CREATION OF AN 'ISSUE'**: Before starting work on a new feature, an issue will be created in our task tracking system (e.g.: ZenHub) to document, discuss, and organize the details of each task, both individually and as a whole.

2. **CREATION OF THE 'FEATURE' BRANCH**: From the `develop` branch, a new feature branch will be created using the command `git checkout -b feature/name-of-the-feature/issue`. _NOTE: after executing this command in the command line, you will automatically switch to the newly created branch._ In this branch, the necessary functionality will be implemented.

3. **PUSHING THE 'FEATURE' BRANCH**: Once the necessary functionality has been implemented in the created feature branch, the modified files will be added to the staging area, a commit will be made in the local repository, and finally, a push will be performed to update the corresponding remote repository branch.

4. **PEER REVIEW**: After completing the previous phase, at least one additional team member must review the changes made in the created feature branch. _Good practice: each modification will be reviewed by as many team members as the effort associated with the issue demands._ This peer review will help ensure, among other things, the quality of the code and/or documentation and its adherence to the established standards.

   Additionally, the peer review will be carried out among members working on related areas of the project.

   Regarding when the peer review should be done, note that once the task is moved to "In Review" with an associated pull request, the team members who need to review it will be notified, as they will also be specifically selected in the associated pull request; the intention is for the reviewers to review the changes as soon as possible, without exceeding 7 days for a single review within the same pull request _(a pull request may require more than one review as reviewers request changes and developers continue working)_.

   Finally, it is important to note that reviewers can perform three types of reviews: (1) COMMENTS, which do not have an explicit approval [this is useful when only recommendations are made or a question is posed to the developer], (2) CHANGE REQUESTS [to be used when the reviewer explicitly asks the developer to change something], and (3) APPROVALS. If a reviewer approves, they will consequently close the pull request and perform the merge.

5. **INTEGRATION INTO THE 'DEVELOP' BRANCH**: After receiving positive feedback from each of the other team members reviewing the changes uploaded to the feature branch, the team member who performed the task may merge the changes into the `develop` branch via merge. _NOTE: it must be stressed that a positive comment must be received; if a negative comment is received, steps 3 and 4 must be repeated as many times as necessary until positive feedback is received from the reviewing team members._

## D.2. How to Prepare Releases

To prepare stable releases of our software, we will follow these steps:

1. **CREATION OF THE RELEASE BRANCH**: From the `develop` branch, a new release branch will be created using the command `git checkout -b release/version-of-release`. In this branch, final tests and corrections will be performed before the final version.

2. **INTEGRATION INTO THE MAIN BRANCH**: Once we are sure that the release version is stable and ready for production, the release branch will be merged into the `main` or `master` branch, which is the primary branch, using a merge.

## D.3. How to Fix Production Bugs

In case errors, issues, or conflicts arise in production after a release, we will address the fix as follows:

1. **CREATION OF A 'HOTFIX' BRANCH**: From the `main` or `master` branch, a hotfix branch will be created using the command `git checkout -b hotfix/name-of-the-error/issue`. In this branch, the identified problem will be resolved.

2. **TESTING AND PEER REVIEW**: After fixing the error, we will ensure the correct functionality of the fix, push the changes to the remote repository, and perform a peer review to ensure its quality and efficiency; if during the peer review the team member receives positive feedback as outlined throughout this document, the next step may proceed.

3. **INTEGRATION INTO BOTH 'MAIN' AND 'DEVELOP' BRANCHES**: The branch created will be merged into both the `main` or `master` branch and the `develop` branch via merges.

<br></br>

# E. Versioning Policies

In our project, we will adopt a semantic versioning approach to clearly and coherently tag and manage software versions. This approach follows the X.Y.Z format, where each number represents a different level of changes in the software:

- **X (Major):** This number represents the primary version of the software and is incremented when significant changes are made that may affect backward compatibility of the API.

- **Y (Minor):** This number denotes the secondary version and is incremented when new features or improvements are added in a backward-compatible manner; note that it may also include minor bug fixes.

- **Z (Patch):** Represents the patch version and is incremented when bug fixes or corrections are made in a backward-compatible manner. These changes are small and do not introduce new features or modify the existing API.

_NOTE: by default, the version number will be incremented after each release, following the aforementioned criteria._

<br></br>

# F. Definition of Done

The development team will consider a task or user story as "Closed" when it has been completed by the team member responsible for that task and has been tested and reviewed or checked by at least one other member. For this, the code or text related to the delivery must have been implemented and pushed by the responsible team member, as well as reviewed and tested by at least one other team member after the task was set to "In Review". If the reviewing team member does not detect any issues, errors, or conflicts and the correct functionality of the code or the proper structure of the document is confirmed, then the project team will consider the task as "Closed", allowing the author to change the task status from "In Review" to "Closed".

<br></br>

# G. Document Management in the Repository

To ensure efficient and organized management of documents generated during the project, such as technical reports, we will adopt a specific structure in our Git repository.

This structure aligns with the previously described branching and versioning strategies, facilitating collaboration and change tracking in the documentation.

All documents generated during the project will be stored in a dedicated folder called `docs`.

This folder will serve as the central repository for all project-related documents and will be located in the root directory of the Git repository.

<br></br>

# Conclusion

Since this is a group project, we have been involved in everything that entails immersion in the Scrum methodology; planning, decision-making, establishing standards and norms to follow throughout the development of the project, among other things.

We have also experienced the organization and commitment required from the entire team to develop this document for its proper development and application.

<br></br>

# Bibliography

[Intentionally left blank]
