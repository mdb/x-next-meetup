# &lt;x-next-meetup&gt;

A [Polymer](http://polymer-project.org) element for displaying a Meetup's next event.

## Usage

1) Import Web Components' polyfill:

```html
<script src="//cdnjs.cloudflare.com/ajax/libs/polymer/0.1.4/platform.js"></script>
```

2) Import custom element:

```html
<link rel="import" href="src/x-next-meetup.html">
```

3) Using it:

```html
<x-next-meetup groupName="YOUR_MEETUP_GROUP" sigId="USER_ID_WHOSE_FEED_YOU_WANT" sig="YOUR_INSTAGRAM_API_ACCESS_TOKEN"></x-next-meetup>
```

This results in unstyled markup:

```html
<h2><a href="http://www.meetup.com/your-group/events/next-event-id/">Next Event Titlte</a></h2>
<time>Tuesday, May 13, 2014, 6:00 pm</time>
<h3><a href="https://www.google.com/maps/place/url+to+event+location+map">Location</a></h3>
<p>555 Street Name, Philadelphia, Pennsylvania</p>
<div class="x-next-meetup-description">
  <p>Your event description.</p>
</div>
<a class="x-next-meetup-rsvp" href="http://www.meetup.com/your-group/events/event-id/">RSVP for Next Event Title</a>
```

What's the `groupName`? The name of your Meetup, as it appears in your group's Meetup URL.

What's a `sigId`? What's a `sig`? Meetup's [API Key signatures](http://www.meetup.com/meetup_api/auth/#keysign) documentation provides a simple overview of how to retrieve these values for use in JavaScript applications.

## Demo

Install dependencies:

Install [Node.js](http://nodejs.org/download/)

Install [Grunt](http://gruntjs.com/):

```sh
$ npm install -g grunt-cli
```

Install Node dependencies:

```sh
$ npm install
```

Install bower dependencies:

```sh
$ bower install
```

Run a local server:

```sh
$ grunt connect
```

Edit the `<x-next-meetup>` element in `index.html`; provide real `sigId`, `sig`, and `groupName` attribute
values. See [Meetup API documentation](http://www.meetup.com/meetup_api/) for more info.

Visit `http://localhost:8000` in your web browser.

## License

[MIT License](http://opensource.org/licenses/MIT)
