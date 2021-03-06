# README
These are the files for 2021 Fantasy Football Developer Kit.

If you're not familiar with Git or GitHub, no problem. Just click the `Source
code` link under the latest release to download the files.  This will download
a file called `fantasy-sdk-2021-vX.X.X.zip`, where X.X.X is the latest version
number.

When you unzip these (note in the book I've dropped the version number and
renamed the directory just `fantasy-sdk-2021`, which you can do too) make note
of where you put them.

For example, on my mac, I have them in my home directory:

`/Users/nathanbraun/fantasy-sdk-2021`

If I were using Windows, it might look like this:

`C:\Users\nathanbraun\fantasy-sdk-2021`

To use these projects, you need to have an ini file called `config.ini`. I've
included an example (`config_example.ini`) for you to use as a starting point.

So the first step is renaming `config_example.ini` to just `config.ini`. Then
you can paste your developer kit license key in it. More details in the PDF
guide.

## Updates & Roadmap (2021-09-09)
Normally, this would have been out earlier in August, however my wife was
diagnosed with Hodgkin's Lymphoma (good prognosis) a few weeks ago. That +
pulling our three kids 5 and under out of school (so they don't get her sick)
has made me crunched for time.

So, while I'm exited about this guide and happy with where it's at, I'm
also releasing it without a few features I wanted to include. However, there
WILL be updates, many in the next few days.

Here are my priorities, most important first:

### Priorities
- [ ] any bug fixes etc that people notice associated with this guide or the
  simulations API; definitely email me — [nate@nathanbraun.com](mailto:nate@nathanbraun.com)
- [X] league integration/analysis/wdis: ability to automatically take into account
  current, midweek scores (will try to do friday after thu night game)
- [X] sleeper integration (hopefully very soon)
- [X] Fantasy Math web access (ditto)
- [ ] a few simulation API convienence improvements
- [ ] typos, clarity etc

Check back here for updated versions. Will keep the changelog updated.

## Changelog
### v0.5.4 and v0.5.5 (2021-10-15)
Remove some misc, unsed imports and fix a few variable references.

### v0.5.3 (2021-10-05)
Bugfix related to the moving the wdis module.

### v0.5.2 (2021-10-04)
Moved the final, auto wdis league integration from
`./projects/integration/wdis_auto_final.py` to `./wdis.py`. Renamed the old
manual version of `./wdis.py` to `./wdis_manual.py`.

### v0.5.1 (2021-10-04)
Minor bugfix to fleaflicker integration code.

### v0.5.0 (2021-09-21)
Added sleeper integration. Like other platforms, uses a snapshot of saved data
that's included here. Should make it easier to follow along.

### v0.4.0 (2021-09-17)
The automatic WDIS and league analysis projects now use a snapshot of saved
data (that I've included in this repository) to make it easier to run through
it and see what I'm seeing.

### v0.3.0 (2021-09-17)
Bugfix - `get_players` utility function now returns ESPN, Yahoo, and Sleeper
IDs.

### v0.2.0 (2021-09-14)
Now includes 2021 Fantasy Math web access. Added instructions for accessing in
book. Basically need to enter you license key at https://fantasymath.com/book

### v0.1.0 (2021-09-13)
Update league integration functions to get midweek points.

E.g. if you were running a WDIS analysis on the Friday after week 1, and your
opponent was starting Gronk, it'd be good to take into account the fact he
scored 29 PPR points the night before. Functions now do that.

Related: saved some snapshots of raw data for the walk throughs to make it
easier to follow along.

### v0.0.4 (2021-09-09)
Make it clearer license keys go in config.ini, not utilities.py. Drop version
numbers from code docstrings — too hard to manually keep up to date.

### v0.0.3 (2021-09-09)
Fix a bug in `./projects/integration/auto_wdis_final`

### v0.0.1 (2021-09-09)
Release!
