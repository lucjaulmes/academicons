# What is Academicons?

Academicons is a specialist icon font for academics. It contains icons for websites and organisations related to academia that are often missing from mainstream font packages. It can be used by itself, but its primary purpose is to be used as a supplementary package alongside a larger icon set. Go [here](http://jpswalsh.github.io/academicons) to view the full icon set along with instructions for their use.

# Requesting new icons

New icons can be requested by creating an issue [here](https://github.com/jpswalsh/academicons/issues). Before submitting a request, please check that the following conditions are satisfied:

  * The organisation in question is already using a logo/icon of appropriate dimensions (roughly square). If that doesn't exist, then there's really not much that can be done, and the request will have to be ignored until such time that a logo/icon can be provided.

  * An icon of appropriate resolution can be provided or linked to. Ideally, the provided file will be a vector file (*e.g.* SVG, EPS, AI) or a PDF with the vector file embedded. These files are all very easy to work with, and result in the most faithful reproductions of the icon. Altenatively, high resolution raster images (*e.g.* JPEG, PNG, GIF) can work, but only if the resolution is high enough that the underlying shapes can be reproduced. Icons made from raster images take much longer to prepare, and require hand drawing each component and figuring out the exact typeface used for any letters. This process can be rather tedious, and I will only do this if there is significant demand for the icon. Favicon files can be useful in conjunction with larger logos that have non-ideal aspect ratios—where they can indicate which part of the logo to strip down to—but they are pretty much useless by themselves. The only time I have made an icon from a favicon was for arXiv, and that was only because: (i) It was heavily requested, and (ii) I was able to get feedback on the new icon from Paul Ginsparg, who made the original icon. You can still submit the request, but it will likely be ignored until someone else comes along and provides the file we need.

  * The icon can be reduced to monochrome. This is one of the basic requirements of a versatile icon, but it is often overlooked when icons are made by people who are not professional designers. Academia is full of unprofessional designers, and it is sometimes the case that a logo relies entirely on the use of different colours. In certain cases we can be creative (see the dblp logo), but more often than not it will be impossible to create a monochrome version of the icon. Again, feel free to make the request, but it will probably be ignored if an alternate logo cannot be found.

You can also directly make a PR for a new icon to be included, see below.

# Adding new icons

To add a new icon with name ${name}, you need to add:
- 1 svg file called `svg/${name}.svg` (use `template.svg` in this repo).
- 1 svg file called `svg/${name}-square.svg` (use `template-square.svg`).
  This should be roughly the same icon as the previous one but white on a black square
- Add the file basenames to `config/codepoints.json` with 2 unused codepoints (ideally next to each other) from the codepage.
  Refer to the [table of which codepoints are currently in use](https://jpswalsh.github.io/academicons/unicode).
- Commit all these changes, and make a PR against the `sources` branch of this repo (should be the one selected by default).

Here is [an example PR](https://github.com/lucjaulmes/academicons/pull/3) so you can see what to expect:
- an automatically generated glyph table diff that shows what the PR changes
- a link to a full and higher resolution glyph table to verify the glyphs render well

# License

- The Academicons font is licensed under the SIL OFL 1.1:
  - [http://scripts.sil.org/OFL](http://scripts.sil.org/OFL)
- Academicons CSS, LESS, and SASS files are licensed under the MIT License:
  - [http://opensource.org/licenses/mit-license.html](http://opensource.org/licenses/mit-license.html)
- The Academicons documentation is licensed under the CC BY 3.0 License:
  - [http://creativecommons.org/licenses/by/3.0/](http://creativecommons.org/licenses/by/3.0/)

# Author

- GitHub: [https://github.com/jpswalsh](https://github.com/jpswalsh)
- Web: [http://jpswalsh.com](http://jpswalsh.com)
