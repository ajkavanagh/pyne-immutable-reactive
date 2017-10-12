# Viewing this presentation

Like some things in life, it's not so easy to view this presentation, as
I took the (somewhat) strange decision to use Jupyter Notebook to actually
make the presentation, along with the
[RISE](https://github.com/damianavila/RISE) extension for a 'live'
presentation.  On the day, it worked out okay, although I actually need to
do something about the default fonts, etc.

## Build a venv with jupyter and RISE

1. You'll need a Python3 installation which can also build extensions.
2. `python3 -m venv <name-of-your-venv>`
3. `source ./<name-of-your-venv>/bin/activate`
4. [Follow](https://github.com/damianavila/RISE) option 2. (because
   I don't like conda on my machines -- no particular reason, to each
   their own):

   * `pip install RISE`
   * `jupyter nbextension install rise --py --sys-prefix`
   * `jupyter nbextension enable rise --py --sys-prefix`

5. `jupyter notebook`

On my Linux machine it was `jupyter-nbextension ...` and on my Mac it was
`jupyter nbextension ...`, so your mileage may vary.

Then just click on the extension.

The repository where I'm experimenting (writing) a reactive framework with
immutable data structures around a very specific topic is:

* https://github.com/ajkavanagh/charms.declarative

Note that it is very much in flux and so may not be the best example of
this technology.  For a more thorough introduction to Reactive programming
and Python, I would suggest [ReactiveX
/ RxPY](https://github.com/ReactiveX/RxPY).
