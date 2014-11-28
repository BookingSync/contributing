# Contributing to BookingSync projects

We'd love to see you contributing to our projects, please just follow a few conventions.

## Coding conventions

- Two spaces, no tabs (for indentation).
- Keep lines fewer than 100 characters.
- No trailing whitespace. Blank lines should not have any spaces.
- Do not indent after private/protected.
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

## Extra Ruby Coding Style

### Methods parenthesis

A method with similar arguments feels right without parenthesis but when passing multiple types ones, please use parenthesis.

```ruby
# Bad
create :foo, bar: baz

# Good
create :foo
create(:foo, bar: baz)
my_method foo, bar
```

### Chaining over multiple lines

You would often want to question yourself if a new method is not best, but if needed,
here's the preferred way to chain methods over multiple lines.

```ruby
# Bad
long_line_under_100_chars.
chained_method()

# Good
long_line_under_100_chars
  .chained_method()
```

# Extra Specs Coding Style

- Add a blank line between `let` and `before`.

## Submiting Pull Requests

- **Fork away** (not required for BookingSync developer team).
- **Create topic branches.** Don't ask us to pull from your master branch.
- **Pull Requests against staging branches.** That's certainly the default behavior on our projects, but if a staging branch is present, base on Pull Requests on it.
- **Migrations.** Make sure to prefix the title with `[migrate]` and add only those changes that are essential for the app to pass tests after migrating. You will have to open a second PR with the rest of your code.
- **Add tests!** Make sure that your patch is including tests.
- **Document any change in behaviour.** Make sure the README and any other relevant documentation are kept up-to-date.
- **Send coherent history.** Make sure each individual commit in your pull request is meaningful. If you had to make multiple intermediate commits while developing, please squash them before sending them to us.

**Note:** In some cases, you might want to submit pull requests for review even before your are done. You might also have pull requests with multiple tasks and progress tracking can be good to share with the rest of the team. In this cases, make a Pull Request early and prefix the subject with `[WIP] `. Pull Requests comments are great to track items completed and left to be done, by using:

```
- [x] Completed super feature
- [ ] Super feature to be done
```

Happy Coding <3
