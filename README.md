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
                <li>Data type: Integer.</li>
            </ul>
            </li>
        </ul>
    </li>
    <li><strong>Response Example</strong> <code>code 200</code>
        <code>
            <pre><span class="pl-kos">[</span>
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
      <span class="pl-kos">{</span>
    <span class="pl-kos">]</span>
  <span class="pl-kos">}</span><span class="pl-kos">,</span>
  <span class="pl-kos">{</span>
    <span class="pl-s">"id"</span>: <span class="pl-s">"5dd5f3a787c49789dca0b43f"</span><span class="pl-kos">,</span>
    <span class="pl-s">"remarks"</span>: <span class="pl-s">"Minim deserunt nisi qui veniam est amet pariatur voluptate ea est exercitation cupidatat sit ea."</span><span class="pl-kos">,</span>
    <span class="pl-s">"pickupTime"</span>: <span class="pl-s">"2018-11-22T07:06:05-08:00"</span><span class="pl-kos">,</span>
    <span class="pl-s">"goodsPicture"</span>: <span class="pl-s">"https://loremflickr.com/320/240/cat?lock=28542"</span><span class="pl-kos">,</span>
    <span class="pl-s">"deliveryFee"</span>: <span class="pl-s">"$104.23"</span><span class="pl-kos">,</span>
    <span class="pl-s">"surcharge"</span>: <span class="pl-s">"$288.13"</span><span class="pl-kos">,</span>
    <span class="pl-s">"route"</span>: <span class="pl-kos">{</span>
      <span class="pl-s">"start"</span>: <span class="pl-s">"Henry Street"</span><span class="pl-kos">,</span>
      <span class="pl-s">"end"</span>: <span class="pl-s">"Clinton Street"</span>
    <span class="pl-kos">}</span><span class="pl-kos">,</span>
    <span class="pl-s">"sender"</span>: <span class="pl-kos">{</span>
      <span class="pl-s">"phone"</span>: <span class="pl-s">"+1 (942) 512-3379"</span><span class="pl-kos">,</span>
      <span class="pl-s">"name"</span>: <span class="pl-s">"Kendra Guthrie"</span><span class="pl-kos">,</span>
      <span class="pl-s">"email"</span>: <span class="pl-s">"kendraguthrie@comdom.com"</span>
    <span class="pl-kos">}</span>
  <span class="pl-kos">}</span><span class="pl-kos">,</span>
  <span class="pl-c">// ...</span>
<span class="pl-kos">]</span></pre>
        </code>
    </li>
</ul>
