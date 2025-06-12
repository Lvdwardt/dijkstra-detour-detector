# Dijkstra's Detour Detector: A GeoJSON Pathfinding Visualizer

Dijkstra's Detour Detector is a lightweight, client-side tool for developers to visually test and debug pathfinding on custom GeoJSON line networks. Upload your network, set start and end points, and instantly see how Dijkstra's algorithm calculates the shortest path. It's perfect for verifying network connectivity, testing routing logic, and demonstrating pathfinding concepts.


## Features for Developers

- **Live Dijkstra Visualization:** See the algorithm's output in real-time on your custom `LineString` network. No server-side setup required.

- **Interactive Testing:** Add, delete, and move waypoints with a single click to dynamically test different routes and edge cases.

- **Visual Debugging:** "Snap lines" instantly show which network nodes are closest to your selected waypoints, helping you identify network gaps or unexpected snapping behavior.

- **GeoJSON I/O:** Load networks via file upload or by pasting raw GeoJSON. Export the resulting path for use in other applications.

- **Framework-Free:** Built with vanilla JavaScript, HTML, and Tailwind CSS for maximum portability and simplicity.


## Development Workflow

This tool is designed to fit into your development and testing workflow, especially when working with custom map data.


### Example Workflow:

1. **Create a Network:** Use a GeoJSON editor like [**vector.rocks**](https://vector.rocks/ "null") or export line data from a GIS tool like QGIS to create your custom network of paths, roads, or corridors.

2. **Export Your Network:** Save the network as a single GeoJSON file containing a `FeatureCollection` of `LineString` features.

3. **Test in the Detector:** Open Dijkstra's Detour Detector and upload your GeoJSON file.

4. **Verify and Debug:** Click various start and end points to see how the algorithm behaves on your network. Use the visual feedback to:

   - Confirm all segments of your network are correctly connected (routable).

   - Check that the calculated paths are logical and efficient.

   - Identify and fix any disconnected islands in your network topology.

This iterative process allows for rapid testing and validation of your map data without needing to integrate a complex routing engine into your main application.


## Technical Details

- **Frontend:** HTML, Tailwind CSS, Vanilla JavaScript

- **Mapping Library:** Leaflet.js

- **Map Tiles:** CartoDB "Voyager"

- **Core Algorithm:** Dijkstra's Algorithm implemented in JavaScript for client-side pathfinding.
