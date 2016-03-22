This jQuery plugin lets you ask your users to tweet before they get access to a download, a discount coupon, etc. 

This plugin is largely based on [this tutorial](http://tutorialzine.com/2011/05/tweet-to-download-jquery/). I've added the cookies support – the plugin now remembers if a visitor has tweeted previously. 

## How to use

Use the following code on your page: 

	$('#tweetLink').tweetAction({
		text: 'Check out this awesome page',
		url: 'https://www.jitbit.com/',
		via: 'jitbit',
		cookies: true
	}, function () {
		// Callback function. Triggered when the user closes the pop-up window:
	}); 

If `cookies` are set to `true` the callback will be executed immediately on all consecutive visits after the first tweet.

## Notes

This plugin is very basic. It assumes that a tweet was published once the modal window is closed. So basically users can just close the window without tweeting and get access to the download. 


Made by [Jitbit](https://www.jitbit.com/)
