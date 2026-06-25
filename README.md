# 9x9 Go Screenshot Scorer

Static browser-only 9x9 Go screenshot scorer.

## Current scoring layer

The app keeps Territory scoring as the default and includes a simple scoring-validation/test layer. It does not include a full Go engine, tactical life-and-death solver, automatic seki solver, or move-search logic.

### Territory scoring

Black = black territory + White stones captured by Black during play + dead White stones marked on board.

White = white territory + Black stones captured by White during play + dead Black stones marked on board + komi.

### Area scoring

Black = live Black stones + Black controlled empty points.

White = live White stones + White controlled empty points + komi.

Prisoners are ignored in Area scoring.

## Developer scoring tests

Open the app in a browser and run this in the console:

```js
runScoringTests()
```

Or open Menu → Advanced → Diagnostics and click **Run scoring tests**.

The test suite covers:

- Empty board with komi only
- Simple Black territory
- Simple White territory
- Neutral/dame region touching both colors
- Dead White stone/group inside Black territory
- Dead Black stone/group inside White territory
- Territory scoring with prisoner input
- Area scoring where prisoners are ignored
- Manual dead-stone marking changes score correctly
- Group in atari is warned but not automatically removed

## Deployment

Upload all files to the root of the GitHub repository and publish through GitHub Pages.
