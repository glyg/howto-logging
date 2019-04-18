python logging howto rewrite


This is a follow-up on the discussion in [python bug tracker issue 28499](https://bugs.python.org/issue28499).

## Ideas (feel free to add to them):

- Both howtos could be a single file (it's the only module with an extra "cook-book" page)

- In the tutorial section of logging.rst, many things are out of place or mixed up.


## Proposed re-write strategy

- [ ] Get a correct structure (based on logging usage)
- [ ] Copy-paste relevant passages from the original doc & cook-book
- [ ] Polish
- [ ] Incite usage of yaml file configuration
- [ ] Add example of "advanced" usages, like `coloredlogs.ColoredFormatter`
- [ ] Sneak in a proposal for a `TRACE` level by giving all the code needed as an example (see [issue 31732](https://bugs.python.org/issue31732))
