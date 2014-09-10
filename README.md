# Contributing to BookingSync projects

We'd love to see you contributing to your projects, please just follow a few conventions.

## Coding conventions

- Two spaces, no tabs (for indentation).
- No trailing whitespace. Blank lines should not have any spaces.
- Indent after private/protected.
- Use Ruby >= 1.9 syntax for hashes. Prefer `{ a: :b }` over `{ :a => :b }`.
- Prefer `&&`/`||` over and/or.
- Prefer `class << self` over `self.method` for class methods.
- Use `a = b` and not `a=b`.
- Prefer `method { do_stuff }` instead of `method{do_stuff}` for single-line blocks.

## Style guides

We code following this style guides:

- [https://github.com/styleguide/ruby](https://github.com/styleguide/ruby)
- [http://betterspecs.org/](http://betterspecs.org/)
- [https://github.com/polarmobile/coffeescript-style-guide](https://github.com/polarmobile/coffeescript-style-guide)
- [https://github.com/airbnb/javascript](https://github.com/airbnb/javascript)

## Submiting Pull Requests

- **Fork away** (not required for BookingSync developer team)
- **Create topic branches.** Don't ask us to pull from your master branch.
- **Pull Requests against staging branches.** That's certainly the default behavior on our projects, but if a staging branch is present, base on Pull Requests on it.
- **Add tests!** Make sure that your patch is including tests.
- **Document any change in behaviour.** Make sure the README and any other relevant documentation are kept up-to-date.
- **Send coherent history.** Make sure each individual commit in your pull request is meaningful. If you had to make multiple intermediate commits while developing, please squash them before sending them to us.

Happy Coding <3
