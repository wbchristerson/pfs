# Readables

<div style="display: flex; flex-direction: column; align-items: center">
    <img alt="A sample image of the post page for an individual post including some comments." width="600" src="../assets/Readables-imgs/post-page.png" style="border: 1px solid #000000;">
    <div style="margin-top: 20px">
        GitHub repository: <a target="\_blank" href="https://github.com/wbchristerson/reactnd-project-readable-starter">https://github.com/wbchristerson/reactnd-project-readable-starter</a>
    </div>
</div>

This project is a forum (content/comment) application in which users may post content to predefined categories, comment on their posts and other users' posts, and vote on posts and comments. The backend server for storing information was provided by Udacity. I made the rest of the application using <code>create-react-app</code> along with React and Redux.

<details>
    <summary>Structure</summary>
    <br>
    <ul>
        <li>On all pages of the application there is a navigation bar listing the name of the application as well as the different post categories. Clicking on a post category will lead the user to a page listing all posts of that category.</li>
        <li>The project opens with a main page listing all currently published posts. There are options at the top of the page for the order of presentation of posts, by date of latest modification as well as by net number of votes. There are also options for composing a new post, with a button that opens a modal for such creation.</li>
        <li>Clicking on any post takes the user to a page for that particular post, listing its data as well as all additional comments.</li>
        <li>Each post itself has a sample avatar image, a title, and content. Content is only visible on the specific post page (not in the main list view). In addition, there are options to edit a post as well as to delete it. Selecting editing will open a modal similar to the composition modal. On the far left side of each post there are also buttons for increasing and decreasing the vote count for a particular post.</li>
        <li>Comments have similar display styles.</li>
    </ul>
</details>

<details>
    <summary>Design</summary>
    <br>
    A view of a sample main page with posts sorted by latest modification:

    <br>

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 30px;">
        <img alt="A sample main page with posts sorted by latest modification." width="500" src="../assets/Readables-imgs/main-page.png" style="border: 1px solid #000000; max-height: 300px;">
    </div>

    A view of a sample page for a specific post together with its associated comments:

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 30px;">
        <img alt="A sample page for a specific post together with its associated comments." width="500" src="../assets/Readables-imgs/post-page-example.png" style="border: 1px solid #000000; max-height: 300px;">
    </div>

    A sample edit modal for a post:

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 30px;">
        <img style="border: 1px solid #000000; max-height: 300px;" alt="A sample edit modal for a post." width="500" src="../assets/Readables-imgs/edit-modal.png">
    </div>
</details>

<details>
    <summary>Running The Application</summary>
    <br>
    To download, you can clone the repository using this terminal command:
    <br>
    <code>git clone https://github.com/wbchristerson/reactnd-project-readable-starter</code>
    <br>
    <br>

    Alternatively, follow the instructions below to download to a hard drive:

    <ul>
        <li>Navigate to <a href="https://github.com/wbchristerson/reactnd-project-readable-starter" target="\_blank">this page</a>.</li>
        <li>Click the green "Clone or download" button towards the right then choose "Download ZIP".</li>
        <li>Find the folder <code>reactnd-project-readable-starter-master</code> in your Downloads folder or wherever it was placed on your device.</li>
        <li>Right click and choose "Extract All".</li>
    </ul>

    To run the application, you will need to have <code>npm</code> installed. See <a href="https://www.npmjs.com/get-npm" target="\_blank">here</a> for installation information. Upon downloading both <code>npm</code> and the project directory, install all dependencies for the API server and execute it from the command line in the project directory by running the following commands in the terminal:
    <br>
    <code>
        cd api-server
        <br>
        npm install
        <br>
        node server
    </code>
    <br>
    <br>

    In another terminal window, run the following commands for the front-end from within the project directory:

    <br>
    <code>
        cd frontend
        <br>
        npm start
    </code>

    <br>
    <br>
    A browser window will open with the project's main page.

    <div style="margin-bottom: 20px;"/>
</details>
