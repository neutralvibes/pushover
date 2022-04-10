# Pushover bash script

Send pushover messages from bash

* Automatically include hostname in title
* Attach images
* Message levels [info|warning|error]
* Assign different sounds to level
* Error level sends high priority messages

## Installation

```bash
wget https://raw.githubusercontent.com/neutralvibes/pushover/master/pushover
chmod +x pushover
```

Now edit the `pushover` file and enter your  `USER_KEY` and `APP_TOKEN`. You can also assign different sounds for the levels.

There is also `HOSTNAME_IN_TITLE` which you can set to `0` to turn off appending the hostname to titles, which is on by default.

## Usage


### Send message

```bash
./pushover info "Test message"
```

### Send message with title

```bash
./pushover info "Test message" "Test title"
```

### Send message with image

```bash
./pushover info "Baby Yoda rocks" "Yodish" babyYodaImage.jpg
```
