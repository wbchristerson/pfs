# Frogger

<div style="display: flex; flex-direction: column; align-items: center">
    <img alt="A sample image of the game screen during use" width="300" src="../assets/Frogger-imgs/general-game.png">
    <div style="margin-top: 20px">
        GitHub repository: <a target="\_blank" href="https://github.com/wbchristerson/arcade-game">https://github.com/wbchristerson/arcade-game</a>
    </div>
</div>

This project re-creates the arcade game Frogger using JavaScript and a basic HTML/CSS skeleton. <a href="https://wbchristerson.github.io/arcade-game/" target="\_blank">Try the game here.</a> Note: This project is based on a skeleton structure from Udacity. For more information, see the initial commit on the appropriate GitHub page given above.

<details>
    <summary>Structure</summary>
    <br>
    <ul>
        <li>The game has 15 levels which the player must complete while avoiding enemy bugs.</li>
        <li>You traverse the board using the arrow keys.</li>
        <li>If you come in contact with a bug, you lose a life and return to the default position on screen.</li>
        <li>You can also collect gems (of varying point values) and stars (which give extra lives).</li>
        <li>If you lose all your lives, the game is over. If you complete all 15 levels with at least one life left, you win.</li>
        <li>When the game ends, you may play again or return to the introductory page.</li>
    </ul>
</details>

<details>
    <summary>Design</summary>
    <br>
    The game begins with an introductory page explaining how to play. It also lists the player's possible avatars, along with which keys to press to switch avatars. Begin by pressing the "space" key.

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px;">
        <img src="/assets/Frogger-imgs/intro-page.png" alt="A screenshot of the game's introductory page" width="300">
    </div>

    The game page includes a background of grass, brick, and water. Your score, remaining lives, and level appear at the bottom. You have to cross the board while avoiding enemy bugs. Gems and stars appear occasionally, and you get points for every gem you collect: 3 for blue gems, 6 for green gems, and 9 for orange gems.

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px;">
        <img src="/assets/Frogger-imgs/game-page.png" alt="A screenshot of the game during play" width="300">
    </div>

    The end page resembles the introductory page and congratulates you on completing the game.

    <div style="display: flex; justify-content: space-around; margin-top: 20px; margin-bottom: 20px; flex-wrap: wrap;">
        <img style="margin-top: 10px; margin-bottom: 10px;" src="/assets/Frogger-imgs/end-lose-page.png" alt="A screenshot of the end page upon a loss" width="300">
        <img style="margin-top: 10px; margin-bottom: 10px;" src="/assets/Frogger-imgs/end-page.png" alt="A screenshot of the end page upon a win" width="300">
    </div>

    <div style="margin-bottom: 20px;">
        The game becomes increasingly difficult. The chance of each of three independent rocks appearing on screen increases up to level 5, after which time they will all always appear (though sometimes overlapping each other). One strategy to avoid losing lives is to wait for the right half of the screen to become clear and cross from that half (since enemy bugs always cross the screen from left to right). To further increase difficulty beyond level 5, a fourth rock will always appear somewhere in the rightmost column.
    </div>
</details>

<details>
    <summary>Running The Application</summary>
    <br>
    Run the application in your browser by <a href="https://wbchristerson.github.io/arcade-game/" target="\_blank">clicking here</a>. To download, clone the repository using this terminal command:
    <br>
    <code>git clone https://github.com/wbchristerson/arcade-game.git</code>
    <br>
    <br>
    Alternatively, follow the instructions below to download to a hard drive:

    <ul>
        <li>Navigate to <a href="https://github.com/wbchristerson/arcade-game" target="\_blank">this page</a>.</li>
        <li>Click the green "Clone or download" button towards the right then choose "Download ZIP".</li>
        <li>Find the folder <code>arcade-game-master</code> in your Downloads folder or wherever it was placed on your device.</li>
        <li>Right click and choose "Extract All" then extract.</li>
        <li>Open your browser and use <code>Ctrl + O</code> (for Windows machines) to open the file selector on your device.</li>
        <li>Go to <code>arcade-game-master</code>, enter <code>arcade-game-master</code> again, then select <code>index.html</code>. The game screen will appear.</li>
    </ul>
</details>
