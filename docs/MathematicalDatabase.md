# Mathematical Database

<div style="display: flex; flex-direction: column; align-items: center">
    <img alt="A sample image of the database main menu" width="300" src="/assets/Mathematical-Database-imgs/database-home.png">
    <div style="margin-top: 20px">
        GitHub repository: <a target="\_blank" href="https://github.com/wbchristerson/database">https://github.com/wbchristerson/database</a>
    </div>
</div>

This project is a small-scale database that uses Python and the graphical user interface package, Tkinter. The database stores solutions to challenging mathematical puzzles and problems drawn from various sources, including mathematical olympiads; however, it can easily be adapted to store other information.

<details>
    <summary>Structure</summary>
    <br>
    The database opens with a menu page and the following buttons: "Look Up An Entry"; "Browse Entries"; "Add An Entry"; and "Edit An Entry".
    <ul>
        <li>"Look Up An Entry" searches for various pieces of information or by an assigned ID. An expanded view for matching data entries is also available.</li>
        <li>"Browse Entries" lists all data entries in both a short form and an expanded view, similar to "Look Up An Entry".</li>
        <li>
            "Write Page" adds data entries. Since the main purpose of the database is to store mathematical puzzles and problems, accepted data include:
            <ul>
                <li>topic</li>
                <li>key words (tags)</li>
                <li>source</li>
                <li>date of completion</li>
                <li>level of difficulty</li>
                <li>problem/puzzle statement (with or without LaTeX formatting)</li>
                <li>solution (with or without LaTeX formatting)</li>
                <li>additional notes</li>
            </ul>
        </li>
        <li>"Edit An Entry" alters information about existing data entries. IDs cannot be changed.</li>
    </ul>

    The project was inspired by <a href="https://artofproblemsolving.com/community/c5h1559064p9530694" target="\_blank">this post</a> by v_Enhance on the website Art of Problem Solving.

    <div style="margin-bottom: 20px;"/>
</details>

<details>
    <summary>Design</summary>
    <br>

    The application begins with the menu shown above. All other page frames have return buttons back to this page. Clicking "Look Up An Entry" brings you to the following frame in the first image below. As mentioned above, you can make queries based on ID in the database or one of the "Add Entry" attributes described above. When the corresponding check box is clicked, an entry widget appears to input data. If no items match the search conditions, then a message to this effect appears in the following text box. Otherwise, a series of search results appears, as seen in the second image below. An "expanded view" check button can be used to toggle between abridged and complete forms of data entries. Warnings will be given for invalid or out-of-range IDs or dates.

    <br>
    <br>

    Note that the "Mentioned Words" and "Source" fields will select entries which match any single searched word (even among many).

    <div style="display: flex; flex-direction: row; justify-content: space-around; flex-wrap: wrap; margin-top: 20px; margin-bottom: 20px;">
        <img style="margin-top: 10px; margin-bottom: 10px;" alt="The Blank Database Search Page" width="300" src="/assets/Mathematical-Database-imgs/database-search-blank.png">
        <img style="margin-top: 10px; margin-bottom: 10px;" alt="The Database Search Page After A Query" width="300" src="/assets/Mathematical-Database-imgs/database-search-data.png">
    </div>

    Clicking "Browse Entries" brings you to the following frame in the first image below. Clicking "Browse" will provide a list of all entries in the database as seen in the second image below. Similar to "Look Up An Entry", clicking the "Expanded View" button will provide more information about items.

    <div style="display: flex; flex-direction: row; justify-content: space-around; flex-wrap: wrap; margin-top: 20px; margin-bottom: 20px;">
        <img style="margin-top: 10px; margin-bottom: 10px;" alt="The Blank Database Browse Page" width="300" src="/assets/Mathematical-Database-imgs/database-browse-blank.png">
        <img style="margin-top: 10px; margin-bottom: 10px;" alt="The Database Browse Page After Browsing" width="300" src="/assets/Mathematical-Database-imgs/database-browse-data.png">
    </div>

    Clicking "Add An Entry" brings you to the following frame in the first image below. The fields for a new data entry match those on the "Look Up An Entry" page, as seen in the second image below. The entry can be cancelled or saved, after which you return to the menu. Warnings are provided for invalid date entries. The collection of all data entries is kept in a JSON file as a list of "DataEntry" objects (which is stored in the form of a list of Python dictionaries for serialization).

    <div style="display: flex; flex-direction: row; justify-content: space-around; flex-wrap: wrap; margin-top: 20px; margin-bottom: 20px;">
        <img style="margin-top: 10px; margin-bottom: 10px;" alt="The Blank Database Write Page" width="300" src="/assets/Mathematical-Database-imgs/database-write-blank.png" style="max-height: 400px;">
        <img style="margin-top: 10px; margin-bottom: 10px;" alt="The Database Write Page After Inputting An Entry" width="300" src="/assets/Mathematical-Database-imgs/database-write-data.png" style="max-height: 400px;">
    </div>

    Clicking "Edit An Entry" brings you to the following frame in the first image below. Input an ID and click "Edit" to update an entry. The fields will be populated with the corresponding data, as shown below in the second image. If the ID is invalid or out of range then a warning appears. Similarly, warnings appear for updating a date to an invalid choice. When finished updating, click the save button. If you do not wish to keep the changes, cancel. In both cases, you will return to the menu page.

    <div style="display: flex; flex-direction: row; justify-content: space-around; flex-wrap: wrap; margin-top: 20px; margin-bottom: 20px;">
        <img style="margin-top: 10px; margin-bottom: 10px;" alt="The Blank Database Edit Page" width="300" src="/assets/Mathematical-Database-imgs/database-edit-blank.png" style="max-height: 400px;">
        <img style="margin-top: 10px; margin-bottom: 10px;" alt="The Database Edit Page After Choosing An Entry To Edit" width="300" src="/assets/Mathematical-Database-imgs/database-edit-data.png" style="max-height: 400px;">
    </div>
</details>

<details>
    <summary>Running The Application</summary>
    <br>
    Python must be installed on your computer to run the application. If you do not have it installed, you can download it for free. For details, see <a href="https://www.python.org/downloads/" target="\_blank">this page</a>. For reference, this project was created using Python version 3.1.
    <br>
    <br>
    If you are running an operating system other than Windows, then you may have to download and install additional software to accommodate the Tkinter toolkit. To learn more or to trouble shoot, see these pages:
    <ul>
        <li><a href="https://www.python.org/download/mac/tcltk/" target="\_blank">https://www.python.org/download/mac/tcltk/</a></li>
        <li><a href="https://wiki.python.org/moin/TkInter" target="\_blank">https://wiki.python.org/moin/TkInter</a></li>
        <li><a href="https://stackoverflow.com/questions/36760839/why-my-python-installed-via-home-brew-not-include-tkinter" target="\_blank">https://stackoverflow.com/questions/36760839/why-my-python-installed-via-home-brew-not-include-tkinter</a></li>
    </ul>
    To download the project, you can clone the repository using this terminal command:
    <br>
    <code>git clone https://github.com/wbchristerson/database.git</code>
    <br>
    <br>
    Alternatively, follow the instructions below to download to a hard drive:
    <ul>
        <li>Navigate to <a href="https://github.com/wbchristerson/database" target="\_blank">this page</a>.</li>
        <li>Click the green "Clone or download" button towards the right then choose "Download ZIP".</li>
        <li>Find the folder <code>database-master</code> in your Downloads folder or wherever it was placed on your device.</li>
        <li>Right click and choose "Extract All".</li>
        <li>Go to <code>database-master</code>, enter <code>database-master</code> again, then double click <code>database.py</code>. The menu will appear.</li>
    </ul>
    Note: The project comes with sample database entries to illustrate how the application works. If you wish to delete these entries and begin with a completely blank database, double click the file <code>delete_database.py</code>. A window will open, prompting you to confirm that you wish to delete all existing entries. To continue, type 'y'. To cancel, type 'n'. For a more aesthetically pleasing presentation of the original problems in the database, see <a href="https://github.com/wbchristerson/database/blob/master/sample_problems.pdf" target="\_blank">sample_problems.pdf</a>.

    <div style="margin-bottom: 20px;"/>
</details>
