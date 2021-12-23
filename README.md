# Inflame the Yellow Crown

Markdown and css used to generate the HTML for https://brstf.itch.io/inflame-the-yellow-crown

CSS was adapted from https://gist.github.com/killercup/5917178

## Pandoc

To re-generate the HTML run

```
pandoc inflame-the-yellow-crown.md --css styles.css -s -o inflame-the-yellow-crown.html
```

I had a problem with the left column of the final table stretching rather than perfectly wrapping its contents. I fixed this by adding a `--columns=1000` following a suggestion from https://github.com/jgm/pandoc/issues/2574. So my final command looked like:

```
pandoc inflame-the-yellow-crown.md --css styles.css -s -o inflame-the-yellow-crown.html --columns=1000
```
