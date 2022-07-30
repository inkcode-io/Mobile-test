# Inkcode Mobidle Developer Technical Challenge 

## Business requirments
As a user i want to be able to see a list of orders, each including a total, a currency, a list of items and an image, along with an address consisting of latitude and longtitude, when i click on an order i want to be able to see it's full information list of items with their prices the address location on the map and the total.

## API Specification
<ul dir="auto">
    <li><strong>Protocol</strong> <code>HTTPS</code></li>
    <li><strong>Hostname</strong> <code>mock-api-mobile.inkcode.io</code></li>
    <li><strong>Method</strong> <code>GET</code></li>
    <li><strong>Endpoint</strong> <code>/v2/orders</code></li>
    <li><strong>Query String Parameters</strong>
        <ul dir="auto">
            <li><code>page</code>
            <ul dir="auto">
                <li>Description: Starting page.</li>
                <li>Items per page: 15</li>
                <li>Data type: Integer.</li>
            </ul>
            </li>
        </ul>
    </li>
    <li><strong>Response Example</strong> <code>code 200</code>
 <pre>
 <span class="pl-kos">{</span>
    <span class="pl-s">"data"</span>: <span class="pl-kos">[</span>
    <span class="pl-kos">{</span>
        <span class="pl-s">"id"</span>: <span class="pl-s">321</span><span class="pl-kos">,</span>
        <span class="pl-s">"total"</span>: <span class="pl-s">15.0000</span><span class="pl-kos">,</span>
        <span class="pl-s">"created_at"</span>: <span class="pl-s">"2014-10-06T10:45:38-08:00"</span><span class="pl-kos">,</span>
        <span class="pl-s">"image"</span>: <span class="pl-s">"https://loremflickr.com/320/240/cat?lock=9953"</span><span class="pl-kos">,</span>
        <span class="pl-s">"currency"</span>: <span class="pl-s">"LBP"</span><span class="pl-kos">,</span>
        <span class="pl-s">"address"</span>: <span class="pl-kos">{</span>
            <span class="pl-s">"lat"</span>: <span class="pl-s">37.412515</span><span class="pl-kos">,</span>
            <span class="pl-s">"lng"</span>: <span class="pl-s">45.215551</span>
        <span class="pl-kos">}</span><span class="pl-kos">,</span>
        <span class="pl-s">"items"</span>: <span class="pl-kos">[</span>
            <span class="pl-kos">{</span>
                <span class="pl-s">"id"</span>: <span class="pl-s">1001</span><span class="pl-kos">,</span>
                <span class="pl-s">"name"</span>: <span class="pl-s">"shoes"</span><span class="pl-kos">,</span>
                <span class="pl-s">"price"</span>: <span class="pl-s">8000.0</span><span class="pl-kos"></span>
            <span class="pl-kos">}</span><span class="pl-kos">,</span>
            <span class="pl-kos">{</span>
                <span class="pl-s">"id"</span>: <span class="pl-s">1003</span><span class="pl-kos">,</span>
                <span class="pl-s">"name"</span>: <span class="pl-s">"skirt"</span><span class="pl-kos">,</span>
                <span class="pl-s">"price"</span>: <span class="pl-s">7000.0</span><span class="pl-kos"></span>
            <span class="pl-kos">}</span><span class="pl-kos"></span>
        <span class="pl-kos">]</span>
    <span class="pl-kos">}</span><span class="pl-kos">,</span>
    <span class="pl-c">// ...</span>
    <span class="pl-kos">],</span>
    <span class="pl-s">"code"</span>: <span class="pl-s">200</span><span class="pl-kos">,</span>
    <span class="pl-s">"message"</span>: <span class="pl-s">"success"</span><span class="pl-kos">,</span>
    <span class="pl-s">"paginate"</span>: <span class="pl-s">{</span><span class="pl-kos"></span>
        <span class="pl-s">"current_page"</span>: <span class="pl-s">1</span><span class="pl-kos">,</span>
        <span class="pl-s">"from"</span>: <span class="pl-s">1</span><span class="pl-kos">,</span>
        <span class="pl-s">"to"</span>: <span class="pl-s">15</span><span class="pl-kos"></span>
        <span class="pl-s">"total"</span>: <span class="pl-s">47</span><span class="pl-kos"></span>
        <span class="pl-s">"per_page"</span>: <span class="pl-s">15</span><span class="pl-kos"></span>
    <span class="pl-kos">}</span>
<span class="pl-kos">}</span>
</pre>
    </li>
</ul>


## Usser Requirments
- retrive a list of orders from the API
- Display that list (order id + formatted date + total + favorite status)
- show order details on a diffrent screen when the user clicks on an order (address on map, items and their prices, total)
- in details screen show a toggle favorite button that adds the order to favorite list or remove it from it depending on it's status, if the user navigates back to orders screen show a favorite indicator (icon) next to the order if it's in favorite list
- favorite status of each order should be presistent

## Technical Requirments
- Source code must be stored on your public Git repository (you can send us the Github link when you finish)
- Other hosting services or zip files are not accepted
- Do not use the name inkcode in naming your Git Repository for the challenge
- Do not copy paste any part of this file
- App should cache orders into local database and can reteive data from the database in case the API call fails (no internet)
- App should implement pagination when calling the API and only load 15 orders at a time and load more when the user reach the end of the screen
- Details screen should implement a map framework (Google Maps, Mapbox) and show a map on the top part of the screen with a marker representing the address
- show notification when the user adds an order to favorites (only when adding)
- play a sound when the user removes an order from favorites (only when removing) (use media player)
- Candidates are free to use any libraries

## Design Requirments
Feel free to use any design you want but the selection of candidates will lean towards the more creative designs if technical skill are matched.


## Areas of assessments
- Usage of clean code
- Architecture
- Code formatting
- Usage of dependency injection
- code reusablity

## Deadline
- 3 Days
- You timer will start exactly 3 hours after the email containing the Test information has been sent to you with the WhatsApp Notification

## Questions
Feel free to contact us Via WhatsApp if you have any questions regading the assigment.
