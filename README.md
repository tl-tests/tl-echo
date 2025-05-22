# TL Echo

A simple Bash script that echoes a provided message a specified number of times, with an optional ability to "shout" the message by converting it to uppercase.
(Purpose of this is just to use the script as a test tool in some other contexts.)

## Usage

```
tl-echo [OPTIONS] message
```

### Options

- `-t, --times <number>`
  Specifies how many times to echo the message. Must be a positive integer. Default is 1.

- `-s, --shout`
  Converts the message to uppercase.

- `-h, --help`
  Displays usage information.

## Examples

Echo a message once (default behavior):

```
tl-echo 'Buy some ice cream.'
```

Output:
```
Buy some ice cream.
```

Echo a message three times:

```
tl-echo --times 3 'Do not forget to buy ice cream.'
```

Output:
```
Do not forget to buy ice cream.
Do not forget to buy ice cream.
Do not forget to buy ice cream.
```

Echo a message in uppercase:

```
tl-echo --shout 'I need ice cream!'
```

Output:
```
I NEED ICE CREAM!
```

Echo a message three times and in uppercase:

```
tl-echo --times 3 --shout 'I really want ice cream! Now!'
```

Output:
```
I REALLY WANT ICE CREAM! NOW!
I REALLY WANT ICE CREAM! NOW!
I REALLY WANT ICE CREAM! NOW!
```

## Notes

Ensure the script has execute permissions:
```
chmod +x tl-echo
```

When running from the same directory, add `./` prefix:
```
./tl-echo 'example message'
```
