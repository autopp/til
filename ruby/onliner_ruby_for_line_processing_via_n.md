# Oneliner ruby for line processing via `-n`

`ruby` provides option `-n`.

If `-n` is set, the given code will be executed as enclosed in the following code:

```ruby
while gets
  # the given code
end
```

The return value of `gets` is stored in `$_`, so this is useful for oneliner excution to line processing.

For example, the following command will output inverse of each line of `input.txt`:

```
$ ruby -n -e 'puts $_.chomp.reverse' < input.txt
```

(This behavior is similar to `awk` or `sed -n`)
