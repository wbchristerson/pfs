# Pixel Art

<div style="display: flex; flex-direction: column; align-items: center">
    <img style="border: 1px solid #000000" alt="A sample creation using this application." width="400" src="/assets/Pixel-Art-Maker-imgs/canvas-example.png">
    <div style="margin-top: 20px">
        GitHub repository: <a target="\_blank" href="https://github.com/wbchristerson/pixel-art">https://github.com/wbchristerson/pixel-art</a>
    </div>
</div>

This project is a one-page application to make colorful pixel images of varying grid sizes. Try the application <a href="https://wbchristerson.github.io/pixel-art/" target="\_blank">here</a>. Note: This project is based on a skeleton structure from Udacity. For more information, see the initial commit on the appropriate GitHub page given above.

<details>
    <summary>Structure</summary>
    <br>
    <ul>
        <li>The dimensions of the pixel grid can each be anything from 1 to 50.</li>
        <li>Once the grid is created, you can choose various colors for the individual pixels.</li>
    </ul>
</details>

<details>
    <summary>Design</summary>
    <br>
    The application is a single page which begins with no shown grid and a default color of black.

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px;">
        <img width="400" style="border: 1px solid #000000" alt="Pixel art maker display before choosing the grid size or color" src="/assets/Pixel-Art-Maker-imgs/canvas-intro.png">
    </div>

    The dimensions of the grid are determined by an input element, which is designed to ensure that you can only enter a number between 1 and 50.

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px;">
        <img width="400" style="border: 1px solid #000000" alt="Pixel art maker display after choosing the grid size but not the color" src="/assets/Pixel-Art-Maker-imgs/canvas-grid.png">
    </div>

    By clicking on the color option, a window appears which shows the various colors that can be generated.

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px;">
        <img width="400" style="border: 1px solid #000000" alt="Pixel art maker display while selecting a canvas color" src="/assets/Pixel-Art-Maker-imgs/canvas-color.png">
    </div>

    Color the grid by clicking on individual pixels:

    <div style="display: flex; justify-content: space-around; margin-top: 20px; margin-bottom: 20px; flex-wrap: wrap;">
        <img width="300" style="border: 1px solid #000000; margin-top: 10px; margin-bottom: 10px;" alt="Pixel art maker display while selecting a canvas color" src="/assets/Pixel-Art-Maker-imgs/canvas-blanket.png">
        <img src="/assets/Pixel-Art-Maker-imgs/canvas-beach.png" alt="Pixel Art Maker Example Image Of Beach" width="300" style="border: 1px solid #000000; margin-top: 10px; margin-bottom: 10px;">
    </div>
</details>

<details>
    <summary>Running The Application</summary>
    <br>
    Run the application in your browser by <a href="https://wbchristerson.github.io/pixel-art/" target="\_blank">clicking here</a>. To download, clone the repository using this terminal command:
    <br>
    <code>git clone https://github.com/wbchristerson/pixel-art.git</code>
    <br>
    <br>
    Alternatively, follow the instructions below to download to a hard drive:

    <ul>
        <li>Navigate to <a href="https://github.com/wbchristerson/pixel-art" target="\_blank">this page</a>.</li>
        <li>Click the green "Clone or download" button above then choose "Download ZIP".</li>
        <li>Find the folder <code>pixel-art-master</code> in your Downloads folder or wherever it was placed on your device.</li>
        <li>Right click and choose "Extract All".</li>
        <li>Open your browser and use <code>Ctrl + O</code> (for Windows machines) to open the file selector on your device.</li>
        <li>Go to <code>pixel-art-master</code>, enter <code>pixel-art-master</code> again, then select <code>index.html</code>. The game screen will appear.</li>
    </ul>
</details>
