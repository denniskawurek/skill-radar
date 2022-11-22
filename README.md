## Setup

1. Get Zalando Tech Radar JS and store it in the root as `radar.js`: [radar.js in Git](https://github.com/zalando/tech-radar/blob/master/docs/radar.js)
2. Get D3.js (version 4.0.0) and store it in the root as `d3.js`:
[D3.js Website](https://d3js.org)
3. Configure your radar. For this you can change the variables in the `index.html`.
For this create a new `Entry` instance. The `Entry` class uses the builder pattern.
Example:

```js
entries.push(
    Entry.init()
        .withLabel("Kibana")
        .inQuadrant(TOOLS.index)
        .inRing(PROFOUND.index)
        .asJSON() // don't forget to call the asJSON function
);
```

If you want other quadrants and rings, just rename them accordingly your needs!