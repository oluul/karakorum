# The Silver Tree of Karakorum

A Three.js miniature diorama of the silver tree fountain in Möngke Khan's palace at Karakorum, capital of the Mongol Empire, as described by the Franciscan friar William of Rubruck, who saw it in 1254.

An angel on top of the tree sounds a trumpet, four gilded serpents pour wine, clarified mare's milk, honey mead and rice wine into silver bowls while silver lions sit at its roots, and a cup-bearer carries a cup up to the Khan while an attendant cries "Uuhai!" and a musician plays.

## Run it

It is a single static page, `index.html`, with no build step. Three.js r160 and the two addons it uses are bundled in `vendor/three/`, the font in `fonts/` and the recitation in the root folder, so the scene itself needs no third-party resources.

Serve the folder with any static server and open it in a browser that supports import maps:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000.

Drag to rotate and scroll to zoom. The scene plays as a silent 16-second loop; press **Listen to the poem** to hear a recitation in Mongolian.

## Historical basis

Every element is checked against a source, and the in-page **Notes & sources** panel marks what is attested and what is inferred.

- **The tree, the hall layout, the court and its customs** follow William of Rubruck's account (W. W. Rockhill's 1900 Hakluyt Society translation, with Peter Jackson's 1990 readings).
- **The floor tiles, granite column bases and wooden columns** follow the Mongolian-German Karakorum Expedition's excavation of the "Great Hall", now identified as a Buddhist temple rather than the palace. Its finds are used only as a contemporary reference.
- **Inferred details** include sizes and proportions, the lions' basins, figure faces and colours, and the composite cast of characters. None of these is described in the sources.

### Sources

- [William of Rubruck's Account of the Mongols (Rockhill translation), Silk Road Seattle](https://depts.washington.edu/silkroad/texts/rubruck.html)
- [German Archaeological Institute (DAI): Conservation and restoration of the "Great Hall of Karakorum"](https://dainst.org/forschung/projekte/noslug/4924)
- [DAI blog: 800 years of Karakorum, 20 years of Mongolian-German excavations](https://www.dainst.blog/?p=7599)
- [Public Domain Review: The Khan's Drinking Fountain](https://publicdomainreview.org/essay/the-khans-drinking-fountain)

## Credits

- [three.js](https://threejs.org/) r160 (MIT licence), bundled in `vendor/three/` with its licence.
- The background waterfall shows the first stanza of *My Native Land* (*Minii nutag*) by Dashdorjiin Natsagdorj (1906–1937), which is in the public domain. It was transcribed from the Cyrillic text into the traditional Mongolian script for this page and has not been checked by a native reader.
- The script is set in a Menksoft typeface (Menksoft Baganatig), bundled as `fonts/zg.ttf`.
- The poem recitation (`Tuuhiinshuleg_audio.m4a`) comes from [this YouTube live stream](https://www.youtube.com/live/8AuyekGnW7E).
- Quotations from Rubruck are from Rockhill's 1900 translation, which is in the public domain.
- All geometry and textures are generated in code; the page uses no external images or models.

## License

[MIT](LICENSE).
