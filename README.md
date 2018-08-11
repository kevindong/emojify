# Emojify
A web app that lets you generate Slack messages consisting of just emojis. This is stupid, but the best kind of stupid.

## Usage
Go [here](https://www.kevindong.net/emojify/) to use the web app. 

**IMPORTANT NOTE**: You **need** to have an emoji called `empty` in your Slack that is a blank white image in order to have the outputted message look right. I have included an `empty.png` file in this repo if you need a blank image. 

If you'd like just the JavaScript function, go into `index.html` and copy paste the `function emojify(emoji, text)` function. Usage for the JS function is self explanatory. If `undefined` is returned, something is wrong with the inputs. Only alphanumeric inputs are accepted for the text. Do not include the colons in the `emoji` parameter.

## Example 1
For the given inputs below:

* `emoji`: `partyparrot`
* `text`: `no typing party parrots only`

the following is generated:

```
:partyparrot::partyparrot::partyparrot::empty::partyparrot::partyparrot::partyparrot:
:partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot:
:partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot:
:partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot:
:partyparrot::empty::partyparrot::empty::partyparrot::partyparrot::partyparrot:

:partyparrot::partyparrot::partyparrot::empty::partyparrot::empty::empty::empty::partyparrot::empty::partyparrot::partyparrot::partyparrot::empty::partyparrot::empty::partyparrot::partyparrot::partyparrot::empty::partyparrot::partyparrot::partyparrot::partyparrot:
:empty::partyparrot::empty::empty::empty::partyparrot::empty::partyparrot::empty::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::empty::empty:
:empty::partyparrot::empty::empty::empty::empty::partyparrot::empty::empty::empty::partyparrot::partyparrot::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::partyparrot:
:empty::partyparrot::empty::empty::empty::empty::partyparrot::empty::empty::empty::partyparrot::empty::empty::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::empty::partyparrot:
:empty::partyparrot::empty::empty::empty::empty::partyparrot::empty::empty::empty::partyparrot::empty::empty::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::partyparrot::partyparrot::partyparrot:

:partyparrot::partyparrot::partyparrot::empty::empty::partyparrot::empty::empty::partyparrot::partyparrot::partyparrot::empty::partyparrot::partyparrot::partyparrot::empty::partyparrot::empty::empty::empty::partyparrot:
:partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::empty::partyparrot::empty::empty::empty::partyparrot::empty::partyparrot::empty:
:partyparrot::partyparrot::partyparrot::empty::partyparrot::partyparrot::partyparrot::empty::partyparrot::partyparrot::empty::empty::empty::partyparrot::empty::empty::empty::empty::partyparrot::empty::empty:
:partyparrot::empty::empty::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::empty::partyparrot::empty::empty::empty::empty::partyparrot::empty::empty:
:partyparrot::empty::empty::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::empty::partyparrot::empty::empty::empty::empty::partyparrot::empty::empty:

:partyparrot::partyparrot::partyparrot::empty::empty::partyparrot::empty::empty::partyparrot::partyparrot::partyparrot::empty::partyparrot::partyparrot::partyparrot::empty::partyparrot::partyparrot::partyparrot::empty::partyparrot::partyparrot::partyparrot::empty::partyparrot::partyparrot::partyparrot:
:partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::empty::partyparrot::empty::empty::partyparrot::empty::empty:
:partyparrot::partyparrot::partyparrot::empty::partyparrot::partyparrot::partyparrot::empty::partyparrot::partyparrot::empty::empty::partyparrot::partyparrot::empty::empty::partyparrot::empty::partyparrot::empty::empty::partyparrot::empty::empty::partyparrot::partyparrot::partyparrot:
:partyparrot::empty::empty::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::empty::partyparrot::empty::empty::empty::empty::partyparrot:
:partyparrot::empty::empty::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::partyparrot::partyparrot::empty::empty::partyparrot::empty::empty::partyparrot::partyparrot::partyparrot:

:partyparrot::partyparrot::partyparrot::empty::partyparrot::partyparrot::partyparrot::empty::partyparrot::empty::empty::empty::partyparrot::empty::empty::empty::partyparrot:
:partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::empty::empty::empty::partyparrot::empty::partyparrot::empty:
:partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::empty::empty::empty::empty::partyparrot::empty::empty:
:partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::empty::empty::empty::empty::empty::partyparrot::empty::empty:
:partyparrot::partyparrot::partyparrot::empty::partyparrot::empty::partyparrot::empty::partyparrot::partyparrot::partyparrot::empty::empty::empty::partyparrot::empty::empty:
```

which in Slack will look like:

![parrots.gif](https://github.com/kevindong/emojify/raw/master/parrots.gif)

## Example 2
For the given inputs below:

* `emoji`: `earth_americas`
* `text`: `hello world`

the following is generated:

```
:earth_americas::empty::earth_americas::empty::earth_americas::earth_americas::earth_americas::empty::earth_americas::empty::empty::empty::earth_americas::empty::empty::empty::earth_americas::earth_americas::earth_americas:
:earth_americas::empty::earth_americas::empty::earth_americas::empty::empty::empty::earth_americas::empty::empty::empty::earth_americas::empty::empty::empty::earth_americas::empty::earth_americas:
:earth_americas::earth_americas::earth_americas::empty::earth_americas::earth_americas::earth_americas::empty::earth_americas::empty::empty::empty::earth_americas::empty::empty::empty::earth_americas::empty::earth_americas:
:earth_americas::empty::earth_americas::empty::earth_americas::empty::empty::empty::earth_americas::empty::empty::empty::earth_americas::empty::empty::empty::earth_americas::empty::earth_americas:
:earth_americas::empty::earth_americas::empty::earth_americas::earth_americas::earth_americas::empty::earth_americas::earth_americas::earth_americas::empty::earth_americas::earth_americas::earth_americas::empty::earth_americas::earth_americas::earth_americas:

:earth_americas::empty::earth_americas::empty::earth_americas::empty::earth_americas::earth_americas::earth_americas::empty::earth_americas::earth_americas::earth_americas::empty::earth_americas::empty::empty::empty::earth_americas::earth_americas::empty:
:earth_americas::empty::earth_americas::empty::earth_americas::empty::earth_americas::empty::earth_americas::empty::earth_americas::empty::earth_americas::empty::earth_americas::empty::empty::empty::earth_americas::empty::earth_americas:
:earth_americas::empty::earth_americas::empty::earth_americas::empty::earth_americas::empty::earth_americas::empty::earth_americas::earth_americas::empty::empty::earth_americas::empty::empty::empty::earth_americas::empty::earth_americas:
:earth_americas::empty::earth_americas::empty::earth_americas::empty::earth_americas::empty::earth_americas::empty::earth_americas::empty::earth_americas::empty::earth_americas::empty::empty::empty::earth_americas::empty::earth_americas:
:earth_americas::earth_americas::earth_americas::earth_americas::earth_americas::empty::earth_americas::earth_americas::earth_americas::empty::earth_americas::empty::earth_americas::empty::earth_americas::earth_americas::earth_americas::empty::earth_americas::earth_americas::empty:
```

which in Slack will look like:

![hello_world.png](https://github.com/kevindong/emojify/raw/master/hello_world.png)

## License
MIT
