# Neighborhood Map

<div style="display: flex; flex-direction: column; align-items: center">
    <img alt="A sample image of a map showing Manhattan Beach, California and listed venues." width="600" src="/assets/Neighborhood-Map-imgs/page-original.png">
    <div style="margin-top: 20px">
        GitHub repository: <a target="\_blank" href="https://github.com/wbchristerson/neighborhood-map">https://github.com/wbchristerson/neighborhood-map</a>
    </div>
</div>

This project includes a neighborhood map of <a href="https://www.citymb.info/" target="\_blank">Manhattan Beach, California</a> along with information about several venues there including local restaurants, ocean-related sites, and stores. The project was bootstrapped with <a href="https://github.com/facebook/create-react-app" target="\_blank">Create React App</a> and developed using <code>React</code>. The map feature used in the application was obtained via <code>react-google-maps</code>, an application that integrates <code>React</code> with Google Maps. In turn, that software was itself based on <a href="https://cloud.google.com/maps-platform/" target="\_blank">Google Maps API</a>. Documentation about <code>react-google-maps</code> can be found <a href="https://github.com/tomchentw/react-google-maps" target="\_blank">here</a>. In addition, the street views for markers that were used were obtained with the <a href="https://developers.google.com/maps/documentation/javascript/streetview" target="\_blank">street view feature</a> of Google Maps, also through <code>react-google-maps</code>. Data about the included venues were extracted using the <a href="https://developer.foursquare.com/" target="\_blank">Foursquare API</a>.

<details>
    <summary>Structure</summary>
    <br>
    <div style="margin-bottom: 20px;">
        The focus of this project is on utilizing APIs to develop an application in conjunction with React.
    </div>
</details>

<details>
    <summary>Design</summary>
    <br>

    Users begin with a map of the neighborhood together with a list view of venues. A search feature allows the user to filter this list and upon clicking any item, the user is taken to the chosen venue's item page, detailing information about the location, hours of operation, busy times of the week and day, a photo view, contact information, customer tips, and more.

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 20px">
        <img alt="A screenshot of the search page" width="500" style="max-height: 400px;" src="/assets/Neighborhood-Map-imgs/filter-page.png" >
    </div>

    Clicking on the corresponding marker on the map will open a street view of the premises. Markers on the map are filtered in accordance with the filtered query and will animate/bounce when the corresponding item is clicked. Additional features include error handling for failed API requests, responsive design for mobile devices, accessibility features for motor- and visually-impaired users in the form of controlled focus, ARIA roles, and alternate image text, and finally, a service worker to cache the data of visited pages in the event of a poor network connection.

    <div style="display: flex; justify-content: center; margin-top: 20px; margin-bottom: 30px">
        <img alt="A screenshot of an individual information page listing data about the venue" width="500" src="/assets/Neighborhood-Map-imgs/information-page.png" style="max-height: 400px;">
    </div>
</details>

<details>
    <summary>Running The Application</summary>
    <br>

    To download, you can clone the repository using this terminal command:
    <br>
    <div style="margin-top: 10px;">
        <code>git clone https://github.com/wbchristerson/neighborhood-map.git</code>
    </div>

    Alternatively, follow the instructions below to download to a hard drive and to run the application:
    <ul>
        <li>Navigate to <a href="https://github.com/wbchristerson/neighborhood-map" target="\_blank">this</a> page.</li>
        <li>Click the green "Clone or download" button towards the right then choose "Download ZIP".</li>
        <li>
            Find the folder <code>neighborhood-map-master</code> in your Downloads folder or wherever it was placed on your device.
        </li>
        <li>Right click and choose "Extract All".</li>
        <li>
            To run the application, you will need to have <code>npm</code> installed. See <a href="https://www.npmjs.com/get-npm" target="\_blank">here</a> for installation information.
        </li>
        <li>
            To install all dependencies for the project from the command line, run the following commands in the terminal from within the project directory:
            <br>
            <code>
                cd neighborhood-map
                <br>
                npm install
            </code>
        </li>
        <li>
            You will need a <code>Google Maps Platform</code> API key along with a <code>Foursquare Client ID</code> and a <code>Foursquare Client Secret</code> to use in the application:
            <ul>
                <li>
                    If you do not have a Google Maps API key already, then you can obtain a <code>Google Maps Platform</code> API key for free <a href="https://cloud.google.com/maps-platform/" target="\_blank">here</a>. You will have to create a billing account but there is a built in $200 credit.
                </li>
                <li>
                    If you do not have the <code>Foursquare Client ID</code> or <code>Foursquare Client Secret</code>, then you can obtain them <a href="https://developer.foursquare.com/" target="\_blank">here</a> by first creating a free account.
                </li>
                <li>
                    After you have all three data items, create a new folder in the <code>src</code> directory called <code>api</code>.
                </li>
                <li>
                    Within <code>api</code>, create a Javascript file called <code>APIkey.js</code>. Within this file add the following lines, where <code>YOUR_GOOGLE_KEY</code>, <code>YOUR_FOURSQUARE_CLIENT_ID</code>, and <code>YOUR_FOURSQUARE_CLIENT_SECRET</code> are replaced by your personalized data values (don't forget the delimiting quotes):
                    <br>
                    <code>
                        export const GOOGLE_MAP_API_KEY = 'YOUR_GOOGLE_KEY'
                        <br>
                        export const FOURSQUARE_CLIENT_ID = 'YOUR_FOURSQUARE_CLIENT_ID'
                        <br>
                        export const FOURSQUARE_CLIENT_SECRET = 'YOUR_FOURSQUARE_CLIENT_SECRET'
                    </code>
                </li>
                <li>Save the file.</li>
            </ul>
        </li>
        <li>
            Assuming that your location in the terminal is now within the <code>neighborhood-map</code> directory, run the following command to execute the application:
            <br>
            <code>npm start</code>
            <br>
            (I believe that <code>yarn start</code> will also be sufficient.)
        </li>
        <li>
            Warning: The service worker that is bundled with <code>create-react-app</code> only works in production mode.
        </li>
    </ul>

    <div style="margin-bottom: 20px;">
        The page will open in the browser.
    </div>
</details>
