# Follow these steps to contribute

**Understand the Project:**

- Familiarize yourself with the project's objectives, architecture, and existing codebase. This will enable you to make informed contributions that align with the project's goals.

**Choose an Issue/Create an issue:**

- Create an issue or work on the existing issue if you're assigned. Also, if you're in `GSSOC'23`, please add `"I'm in GSSOC'23"` so that we can add the `GSSOC'23` label on that particular issue/PR.

**Assign an Issue Number:**

- Assign the `#ISSUE_NUMBER` in the description of the PR request.

**Work on Your assigned issue first:**

- We kindly request that you prioritize working on your assigned issue at this time. It is highly recommended that you begin by creating an issue before proceeding to create a pull request.
- By doing so, you can outline the problem or task at hand and facilitate a smoother workflow.
- Once the issue is established, please proceed to implement the necessary changes, address any bugs, or incorporate new features to effectively resolve the selected issue/task.

**Commit Your Changes:**

- Once you have made significant progress or completed your contribution, commit your changes with a descriptive commit message.
- It is advisable to make frequent, small commits to make the review process more manageable. Please check [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/)

## DO NOT SPAM !!! ⚠

- If the manatainer or owner finds any blank issue or any kind of unethical behaviour from a certain individual.
- The individual will labeled as `SPAM` and will be prohibited from any kind of contribution or participation in future in this project.

# How to add your projects to ProjectsHut

#### 1. Fork this repository

![ Fork this repository](https://user-images.githubusercontent.com/88102392/226444075-7d7d28b5-8d88-459a-bb82-38a3f64aaf28.png)

#### 2. Click on `Go to file`

![Go to file](https://user-images.githubusercontent.com/88102392/226444608-12a2abb9-436c-4843-8893-49029cb4c033.png)

#### 3. Add following code to end of `src/DB/projects.json`

```json
{
  "github_username": "YOUR_GITHUB_USERNAME",
  "Social_media": {
    "gitHub": "YOUR_GITHUB_ACCOUNT_LINK",
    "LinkedIn": "YOUR_LINKEDIN_ACCOUNT_LINK",
    "Instagram": "YOUR_INSTAGRAM_ACCOUNT_LINK",
    "YouTube": "YOUR_YOUTUBE_ACCOUNT_LINK",
    "Twitter": "YOUR_TWITTER_ACCOUNT_LINK"
  },
  "Projects": [
    {
      "link": "PROJECT_LINK",
      "title": "PROJECT_NAME",
      "description": "PROJECT_DESCRIPTION",
      "tech": ["tech1", "tech2"]
    },
    {
      "link": "PROJECT_LINK",
      "title": "PROJECT_NAME",
      "description": "PROJECT_DESCRIPTION",
      "tech": ["tech1", "tech2"]
    }
  ]
}
```

You should write the full Tech name: <br>
**👎 Bad Tech Names:** js, JS, react, reactjs, css <br>
**👍 Good Tech Names:** Javascript, ReactJS, CSS

#### 4. Commit all changes.

- Add a commit like this for only projects addition `data: project addition by [your-githubuser-name] #issue_number`

> ### Alternatively, if you prefer to run the project locally, follow these steps:

1.  Go to preferred folder in your computer and paste the following command after forking our repository (Only one of it if you don't have ssh setup then go with HTTP command)

    - HTTP
      `git clone https://github.com/<YOUR-USERNAME>/ProjectsHut.git`
    - SSH
      `git clone git@github.com:<YOUR-USERNAME>/ProjectsHut.git`

2.  Navigate to the project folder

    ```
    cd ProjectsHut
    ```

3.  Install dependencies

    ```
    pnpm i
    ```

4.  Now do ahead and create a new branch and move to the branch

    ```
    git checkout -b fix-issue-<ISSUE-NUMBER>
    ```

5.  Run in local

    ```
    pnpm dev
    ```

6.  Make sure all the test cases pass

    ```
    pnpm test
    ```

7.  After done you can now push this changes, for doing that follow the following command chain

    - `git status` (Shows the changed files)
    - `git add .` (Will add all the files to staging area)
    - `git commit -m "feat/docs/fix: <EXPLAIN-YOUR_CHANGES>"`
    - > If you encounter this error while commits
      >
      > ```diff
      > husky - pre-commit hook exited with code 1(error)
      > ```
      >
      > use this command
      >
      > ```diff
      > pnpm format
      > ```
    - `git remote add upstream https://github.com/priyankarpal/ProjectsHut.git`
    - `git push origin fix-issue-<ISSUE-NUMBER>`

8.  After this go to your forked GitHub repository and go to `Pull Request` section. Now you might be able to see a pop up saying **Pull Request**. Click on the popup and you will be redirected to pull request page

9.  Now fill in the form template of the pull request and give the necessary description.

10. Click on **Submit**

11. Hurray! You just made your first contribution to this project 🎉

12. Wait for your pull request to be reviewed and merged.

> NOTE: Please make sure to follow the [Code of conduct](https://github.com/priyankarpal/ProjectsHut/blob/main/CODE_OF_CONDUCT.md) while contributing.

## Useful Links

- [GitHub Forking Guide](https://docs.github.com/en/get-started/quickstart/fork-a-repo)
- [GitHub Pull Requests Guide](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests)
- [GitHub Issues Guide](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues)
- [Contributor Covenant Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/)
