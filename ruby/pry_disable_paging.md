### Pager

`Pry.config.pager` is a boolean option determining whether a pager
will be used for long output. Setting it to `false` disables the
pager.

Currently only the `less` pager is supported, though a very simple
custom pager is used if `less` is not available.

It may be necessary to turn paging off if you are running Pry from within
an emacs shell or similar.

**Default value:** `true`

Example: Disabling paging

Permanently (in a .pryrc file)
```ruby
Pry.config.pager = false
```
Temporarily (in a repl session)
```ruby
_pry_.config.pager = false
```
