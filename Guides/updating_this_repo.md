# How to update this repository

## Open the repository where you can make edits

This can be done in at least three different ways:

> [!IMPORTANT]
> For all of the following methods, make sure you create a new branch for your changes, and do not commit directly to the `main` branch. This is important to ensure that your changes can be reviewed and merged properly. See the [section below](#how-to-create-a-new-branch) on how to create a new branch.

1. Clone the repository to your local machine, or cd into the repository if you already have it cloned
> [!TIP]
> If you're not familiar with the command line, you can use an editor like VSCode or PyCharm to open the repository and use their built-in terminal, or their GUI. Make sure you have Git installed, and the Git extension installed in your editor for better integration.
    - If you're using VSCode, you can open the repository by selecting "Open Folder"
          and navigating to the repository directory. The built-in terminal can be accessed via `View > Terminal`.
    - If you're using the terminal, you can use the following commands:
        - `git clone <repository-url>` to clone the repository
        - `cd <repository-name>` to change into the repository directory
        - `git pull` to ensure you have the latest changes from the remote
        - `git status` to check the status of your repository
        - `git branch` to check which branch you are currently on. You should not be on the `main` branch when making changes.

2. Use the GitHub web interface to edit files directly in the repository
    - Navigate to the file you want to edit, click on the pencil icon to edit the file
    - Make your changes and commit them directly in the web interface. Make sure you do not commit to the `main` branch directly.
    - Use the "Propose changes" button to create a pull request
    - This is useful for small changes or quick fixes

3. Use GitHub codespaces to edit files in the repository in the browser
    - Navigate to the repository and click on the "Code" button
    - Select "Open with Codespaces" to create a new codespace
    - This allows you to edit files in a full development environment in the browser
    - Make your changes and commit them directly in the codespace, either using the terminal or the built-in editor (see terminal instructions above)

## How to create a new branch

> [!TIP]
> Use a descriptive name for the branch, using your initials as a prefix such as `hs_pre-august-session-2023`

Several options here depending on how you are editing the repository:

1. In the terminal, use the command `git checkout -b <branch-name>` to create and switch to the new branch.

2. In the GitHub web interface, you can create a new branch by clicking on the branch selector dropdown and typing in a new branch name. Make sure to select the base branch as `main` and then click "Create branch". This can also be done after you have made changes to a file and clicked "Propose changes" in the web interface.

3. In GitHub codespaces, you can create a new branch using the terminal as described above, or by using the branch selector dropdown in the top left corner of the editor. Type in a new branch name and press Enter to create it.

## What changes to make

### Before a session

> [!NOTE]
> Before making changes ahead of a session, make sure a sign-up form/event has been created and is shareable. See more information on this in our [organising guide](./organising.md).

- Copy the [`session-template.md`](../Sessions/session-template.md) to `Sessions/YEAR/MM-YY-session.md`, using the year and month the session will take place.
  - For example, if the session is in August 2023, the file should be named `Sessions/2023/08-23-session.md`
  - Make sure to create the `Sessions/YEAR` directory if it does not already exist
- Update the sections of the template in ALL-CAPS
  - These sections are meant to be filled in with the relevant information for the session
  - Make sure to remove the ALL-CAPS text once you have filled in the section
  - You can add the link to the content and the event at the bottom of the file, in the "Links" section
- Update the session date and link to the new file with details in the [`README.md` file](../README.md/#next-session) and the [`SESSIONS.md` file](../SESSIONS.md/#upcoming-sessions)

### After a session

- Remove the sign-up form/event link from the [`README.md` file](../README.md/#next-session), the `MM-YY-session.md` file and the [`SESSIONS.md` file](../SESSIONS.md/#upcoming-sessions) if it's on there.
- Move the details of the session in the [`SESSIONS.md` file](../SESSIONS.md) to the ["Previous Sessions" section](../SESSIONS.md/#previous-sessions).
