# My Reads

<div style="display: flex; flex-direction: column; align-items: center">
    <img alt="A sample image of the bookshelves showing cover illustrations and titles for selected books." width="500" src="/assets/My-Reads-imgs/main-page.png" style="border: 1px solid #000000;">
    <div style="margin-top: 20px">
        GitHub repository: <a target="\_blank" href="https://github.com/wbchristerson/reactnd-project-myreads-starter">https://github.com/wbchristerson/reactnd-project-myreads-starter</a>
    </div>
</div>

This application keeps track of a user's book selections from a static database on a server. The user may query certain topics and then select books from the search results to appear on one of three shelves on the main page: "Currently Reading", "Want To Read", and "Read". The project was completed using React, with a basic template and server provided by Udacity.

<details>
    <summary>Structure</summary>
    <ul>
        <li>The main page displays the set of books selected. Such books are shown in three sections on the main page, distinguished by whether the user has read, is reading, or will read a given book.</li>
        <li>The search page provides a section to look up a specific topic (limited to certain queries) and will update results as search items are typed.</li>
        <li>Books in both the bookshelves page and the search page have associated buttons to add or remove them from bookshelves as well as to toggle between bookshelves.</li>
    </ul>
</details>

<details>
    <summary>Design</summary>
    <br>
    The main page is composed of three sections for "currently reading", "want to read", and "read".

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px;">
        <img alt="A sample view of the main page showing three bookshelves with images of book covers, titles, and authors." src="/assets/My-Reads-imgs/full-page.png" width="500" style="border: 1px solid #000000; max-height: 300px;">
    </div>

    You can also add many books to a single section.

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px;">
        <img alt="A close up view of the 'currently reading' section with many books appearing in the form of book covers with titles and authors." src="/assets/My-Reads-imgs/many-books.png" width="500" style="border: 1px solid #000000; max-height: 300px;">
    </div>

    Selections can be modified by clicking on the arrow item for a single book.

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px;">
        <img alt="A view of a row of books with the selection tab open for one of the books, providing options for moving that book." src="/assets/My-Reads-imgs/entry-click.png" width="500" style="border: 1px solid #000000; max-height: 300px;">
    </div>

    The search page appears in a similar manner. Type in a search option and see the results that appear.

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px;">
        <img alt="The Blank Database Write Page" src="/assets/My-Reads-imgs/search-page.png" width="500" style="border: 1px solid #000000; max-height: 300px;">
    </div>
</details>

<details>
    <summary>Running The Application</summary>
    <br>
    To download, you can clone the repository using this terminal command:
    <br>
    <code>git clone https://github.com/wbchristerson/reactnd-project-myreads-starter.git</code>

    <br>
    <br>
    Alternatively, follow the instructions below to download to a hard drive:
    <ul>
        <li>Navigate to <a href="https://github.com/wbchristerson/reactnd-project-myreads-starter" target="\_blank">this page</a>.</li>
        <li>Click the green "Clone or download" button towards the right then choose "Download ZIP".</li>
        <li>Find the folder <code>reactnd-project-myreads-starter</code> in your Downloads folder or wherever it was placed on your device.</li>
        <li>Right click and choose "Extract All"</li>
    </ul>

    To run the application, you will need to have <code>npm</code> installed. See <a href="https://www.npmjs.com/get-npm" target="\_blank">here</a> for installation information. Upon downloading both <code>npm</code> and the project directory, install all project dependencies by running the following command from within the project directory:
    <br>
    <code>npm install</code>
    <br>
    <br>
    Afterwards, start the development server with this command:
    <br>
    <code>npm start</code>
    <br>
    <br>
    A browser window will open with the main page.

    <div style="margin-bottom: 20px;"/>
</details>
