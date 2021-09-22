# Mobile Flashcards

<div style="display: flex; flex-direction: column; align-items: center">
    <img alt="A sample image of the list of all flashcard decks that have been created" width="200" src="../assets/Mobile-Flashcards-imgs/main-page.png">
    <div style="margin-top: 20px">
        GitHub repository: <a target="\_blank" href="https://github.com/wbchristerson/MobileFlashcards">https://github.com/wbchristerson/MobileFlashcards</a>
    </div>
</div>

This project is a flashcard application for Android mobile devices in which users may create collections of flashcards and quiz themselves on the decks that they compile. I created the application using <code>react-native</code> along with <code>redux</code>. (This project was bootstrapped with <a href="https://github.com/react-community/create-react-native-app" target="\_blank">Create React Native App</a>.)

<details>
    <summary>Structure</summary>
    <br>
    <ul>
        <li>The main section includes a tab navigator for flashcard decks that have already been created as well as a tab for creating new decks.</li>
        <li>Clicking on a deck tile takes the user to the individual page for the topic, where additional cards for the deck can be created and added.</li>
        <li>From the individual deck page, users may also take quizzes in which they mark their responses based on the answers shown. Afterwards, a score is given.</li>
    </ul>
</details>

<details>
    <summary>Design</summary>
    <br>
    As said above, the application begins with a tab navigator composed of two screens. The first is a list view of all currently available flashcard decks. As a starting point, two decks are already provided: "Spanish" (9 cards) and "Architecture" (2 cards) . You may quiz yourself with these or add new decks.

    <br>
    <br>

    The second screen in the tab navigator is a form to add an additional deck ("new deck"). Submitting the form will take the user to the new page for that deck.

    <br>
    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px;">
        <img alt="A screenshot of the game's new deck page" width="200" style="max-height: 400px;" src="/assets/Mobile-Flashcards-imgs/new-deck.png">
    </div>

    Individual deck pages can be reached by clicking on a deck from the list view. This lists the name of the deck, the number of cards, and buttons for adding a card to the deck as well as for quizzing one's self.

    <br>
    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px;">
        <img alt="A screenshot of the app's individual deck page" width="200" style="max-height: 400px;" src="/assets/Mobile-Flashcards-imgs/deck.png">
    </div>

    The "new card" form is similar to the "new deck" form.

    <br>
    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px;">
        <img alt="A screenshot of the app's new card page" width="200" style="max-height: 400px;" src="/assets/Mobile-Flashcards-imgs/new-card.png">
    </div>

    The quiz page displays the deck questions in order with an available button to check the answer and then grade one's self. Clicking the answer field will reveal the answer to the given question. When the user finishes looking through the deck, his/her score is shown.

    <br>
    <div style="display: flex; justify-content: space-around; margin-top: 20px; margin-bottom: 20px; flex-wrap: wrap;">
        <img style="margin-top: 10px; margin-bottom: 20px; border: 1px solid #000000" alt="A screenshot of the app's question page" src="/assets/Mobile-Flashcards-imgs/quiz-question.png" width="200" style="border: 1px solid #000000; max-height: 400px;">
        <img style="margin-top: 10px; margin-bottom: 20px; border: 1px solid #000000; max-height: 400px;" alt="A screenshot of the app's question page with an answer" src="/assets/Mobile-Flashcards-imgs/quiz-answer.png" width="200">
        <img style="margin-top: 10px; margin-bottom: 20px; border: 1px solid #000000; max-height: 400px;" alt="A screenshot of the app's score result page" src="/assets/Mobile-Flashcards-imgs/finished-quiz.png" width="200">
    <div>

    To maintain data for this application, I used the <code>AsyncStorage</code> key-value storage system heavily.
</details>

<details>
    <summary>Running The Application</summary>
    <br>
    <br>
    To download, you can clone the repository using this terminal command:
    <code>git clone https://github.com/wbchristerson/MobileFlashcards.git</code>

    <br>
    <br>

    Alternatively, follow the instructions below to download to a hard drive:

    <ul>
        <li>Navigate to <a href="https://github.com/wbchristerson/MobileFlashcards" target="\_blank">this</a> page.</li>
        <li>Click the green "Clone or download" button towards the right then choose "Download ZIP".</li>
        <li>Find the folder <code>MobileFlashcards-master</code> in your Downloads folder or wherever it was placed on your device.</li>
        <li>Right click and choose "Extract All" then extract.</li>
    </ul>

    In all cases, having downloaded the files:

    <ul>
        <li>
            To install all dependencies from the command line, run the following command in the terminal within the project folder:
            <br>
            <code>npm install</code>
        </li>
        <li>
            In another terminal window, run the following command to start the project:
            <br>
            <code>npm start</code>
        </li>
    </ul>

    The terminal will then provide you with several options. If you have the application <a href="https://expo.io/" target="\_blank">Expo</a> on your device, then you can scan the accompanying QR code that appears. This will give you the option to run the application on mobile (note: the scan is most easily executed on terminals with a black background and a gray or white foreground).

    <br>
    <br>

    For complete details about running react-native applications such as this one on mobile devices, see <a href="https://facebook.github.io/react-native/docs/running-on-device" target="\_blank">here</a>.

    <div style="margin-bottom: 20px;"/>

</details>
