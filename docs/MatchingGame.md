# Matching Game

<div style="display: flex; flex-direction: column; align-items: center">
    <img alt="A sample image of the matching game during use" width="400" src="/assets/Matching-Game-imgs/display.png">
    <div style="margin-top: 20px">
        GitHub repository: <a target="\_blank" href="https://github.com/wbchristerson/memory-game">https://github.com/wbchristerson/memory-game</a>
    </div>
</div>

Using HTML, CSS, and JavaScript, this two-page application challenges the player to find all matching pairs of cards in the fewest moves. To try the game, <a href="https://wbchristerson.github.io/memory-game/" target="\_blank">click here</a>. Note: This project is based on a skeleton structure from Udacity. For more information, see the initial commit on the appropriate GitHub page given above.

<details>
    <summary>Structure</summary>
    <br>
    <ul>
        <li>You must find the 8 matching images from cards that are turned over.</li>
        <li>When you click a card, it flips, turns blue, and the hidden image appears.</li>
        <li>When you make a match, the cards change color and the images remain visible.</li>
        <li>If you do not make a match, the cards flip back over to their original display.</li>
        <li>Once you match all cards, the game is over and the screen congratulates you, listing various statistics about your game. To play again, click the "play again" button.</li>
    </ul>
</details>

<details>
    <summary>Design</summary>
    <br>
    The main screen includes a timer, a move counter, a reset button, and a star rating. Below is an example of the interface:

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px;">
        <img width="400" src="/assets/Matching-Game-imgs/memory-game-page.png" alt="A screenshot of the game's introductory page" style="max-height: 400px;">
    </div>

    Finishing with at most 15 moves yields a 3-star rating, finishing with more than 16 moves but at most 25 yields a 2-star rating, and finishing with more than 25 moves yields a 1-star rating. Here is an example end page:

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px;">
        <img width="400" src="/assets/Matching-Game-imgs/memory-end-page.png" alt="A screenshot of the game's end page">
    </div>
</details>

<details>
    <summary>Running The Application</summary>
    <br>
    Run the application in your browser by <a href="https://wbchristerson.github.io/memory-game/" target="\_blank">clicking here</a>. To download, clone the repository using this terminal command:
    <br>
    <code>git clone https://github.com/wbchristerson/memory-game.git</code>
    <br>
    <br>
    Alternatively, follow the instructions below to download to a hard drive:
    <ul>
        <li>Navigate to <a href="https://github.com/wbchristerson/memory-game" target="\_blank">this page</a>.</li>
        <li>Click the green "Clone or download" button towards the right then choose "Download ZIP".</li>
        <li>Find the folder <code>memory-game-master</code> in your Downloads folder or wherever it was placed on your device.</li>
        <li>Right click and choose "Extract All" then extract.</li>
        <li>Open your browser and use <code>Ctrl + O</code> (for Windows machines) to open the file selector on your device.</li>
        <li>Go to <code>memory-game-master</code>, enter <code>memory-game-master</code> again, then select <code>index.html</code>. The game screen will appear.
        </li>
    </ul>
</details>
