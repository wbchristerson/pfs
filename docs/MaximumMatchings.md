# Maximum Matchings

<div style="display: flex; flex-direction: column; align-items: center">
    <img alt="Image of the result of the algorithm" width="500" src="/assets/Maximum-Matchings-imgs/main-sample-large.png">
    <div style="margin-top: 20px">
        GitHub repository: <a target="\_blank" href="https://github.com/wbchristerson/perfect-matchings">https://github.com/wbchristerson/perfect-matchings</a>
    </div>
</div>

This application demonstrates an algorithm for finding maximum matchings in bipartite graphs. The general procedure used begins with finding any maximal matching greedily, then expanding the matching using augmenting paths via almost augmenting paths. For a detailed explanation of the concepts involved, see <a href="https://github.com/wbchristerson/perfect-matchings/blob/master/Maximum_Matchings.pdf" target="\_blank">Maximum_Matchings.pdf</a>. The user can choose the bipartite graph in various ways or add edges randomly. There is then a series of selection options for demonstrating the algorithm. This project was created using Python along with the pygame and livewires packages.

<details>
    <summary>Structure</summary>
    <br>
    <ul>
        <li>The user may navigate through the various pages to choose the bipartite graph examined.</li>
        <li>There are options to choose the sizes of the branches as well as which edges appear. Alternatively, edges can be chosen for the user randomly.</li>
        <li>There are then options for attempting to find a maximum matching manually, as well as for immediately displaying a maximum matching. In addition, the user may watch the application of the algorithm continuously or with steps.</li>
    </ul>
</details>

<details>
    <summary>Design</summary>
    <br>
    To navigate throughout the pages of the program, there are buttons which can be hovered over. To push the buttons you must push the space bar while hovered over, rather than clicking.

    The application begins with a page for selecting the left branch size.

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px">
        <img alt="Left branch selection view" width="400" src="/assets/Maximum-Matchings-imgs/left-selection.png" >
    </div>

    This is followed by a similar page for selecting the right branch size.

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px">
        <img alt="Right branch selection view" width="400" src="/assets/Maximum-Matchings-imgs/right-selection.png">
    </div>

    The user may then elect to choose edges manually or to allow the program to randomly select edges, adding any individual edge using a pseudo-random number generator with probability 40%. Below is a view for making edge selections manually.

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px">
        <img alt="Edge selection view" width="400" src="/assets/Maximum-Matchings-imgs/edge-selection.png">
    </div>

    The user is then taken to a page for selecting the type of operation to apply.

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px">
        <img alt="Operations options view" width="400" src="/assets/Maximum-Matchings-imgs/operation-options.png">
    </div>

    Upon selecting the manual matching option, the user is allowed to select edges of the graph to try to find a maximum matching. Congratulations are given upon succeeding.

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px">
        <img alt="Manual matching view" width="400" src="/assets/Maximum-Matchings-imgs/manual-match.png">
    </div>

    After selecting the automatic matching option, a maximum matching is immediately displayed.

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px">
        <img alt="Automatically generated maximum matching displayed" width="400" src="/assets/Maximum-Matchings-imgs/match-automatic.png">
    </div>

    If the user selects the option to watch the algorithm, the steps of the algorithm will be displayed with changes occurring every few seconds (with a pause button available). The first image below is a still of the initial greedy matching generation and the second image below is a still of the identification of an augmenting path to increase the size of the matching.

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px">
        <img alt="Greedy matching search view" width="400" src="/assets/Maximum-Matchings-imgs/matching-watch-A.png">
    </div>

    <div style="display: flex; justify-content: center; margin-bottom: 20px;">
        <img alt="Identification of an augmenting path" width="400" src="/assets/Maximum-Matchings-imgs/matching-watch-B.png">
    </div>

    The fourth option also displays the steps of the algorithm but with buttons to follow the steps.

    <div style="margin-top: 20px"></div>
</details>

<details>
    <summary>Running The Application</summary>
    <br>
    You will need to have Python installed, as well as the pygame and livewires libraries. The version of livewires used for this project was taken from this <a href="http://www.delmarlearning.com/companions/content/1435455002/downloads/index.asp?isbn=1435455002" target="\_blank">download</a> (which also contains downloads for Python and pygame), under "Book related software". To download Python only, visit this <a href="https://www.python.org/downloads/" target="\_blank">page</a>.

    <br>
    <br>

    To download, clone the repository using this terminal command:<br>
    <code style="margin-top: 20px;">git clone https://github.com/wbchristerson/perfect-matchings.git</code>

    <br>
    <br>
    Alternatively, follow the instructions below to download to a hard drive:
    <ul>
        <li>Navigate to <a href="https://github.com/wbchristerson/perfect-matchings" target="\_blank">this page</a>.</li>
        <li>Click the green "Clone or download" button towards the right then choose "Download ZIP".</li>
        <li>Find the folder <code>perfect-matchings-master</code> in your Downloads folder or wherever it was placed on your device.</li>
        <li>Right click and choose "Extract All" then extract.</li>
        <li>From within the directory generated through extraction (named <code>perfect-matchings-master</code>, unless you changed the file name), double click on the batch file <code>main.bat</code>. A window will open on screen, beginning the program.</li>
    </ul>
    If you encounter errors involving <code>pygame</code> or <code>livewires</code>, make sure that those packages are installed in <code>lib/site-packages</code> from the level of the directory containing this project.

    <div style="margin-top: 20px"></div>
</details>
