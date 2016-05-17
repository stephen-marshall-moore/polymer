# Polymer

Polymer is a web components material design theme for [Hugo](http://gohugo.io/).
This fork of the project is probably not very mergeable/pullable back to the original by pdevty, for better or for worse, blame stephen.

![](https://github.com/stephen-marshall-moore/polymer/blob/master/images/tn.png)

## Features

- Material Design by [polymer](https://www.polymer-project.org/1.0/)
- Google Analytics (optional)
- Pagination
- Disqus (optional)
- Twitter, Facebook, GitHub, Google+, LinkedIn links (optional)
- Tags
- Categories
- Cover, Photo, Profile image (optional)
- Highlighting source code

## Installation

```shell
$ mkdir themes
$ cd themes
$ git clone https://github.com/stephen-marshall-moore/polymer
```

## Usage

```shell
$ hugo server -t polymer -w -D
```

## Configuration

config.json

```json
{
	"theme": "polymer",
	"baseurl": "http://blog.nimbostrati.com",
	"languageCode": "en-us",
	"title": "Blog Nimbostrati",
	"MetaDataFormat": "json",
	"paginate": 10,
	"disqusShortname": "Your Optional Disqus Name",
	"copyright": "© 2015 Copyright Text",
	"params": {
		"author": "Stephen Moore",
		"photo": "images/photo.png",
		"profile": "images/profile.png",
		"cover": "images/cover.png",
		"logos": [
			{
				"site": "weibo",
				"username = "Your Weibo name"
			},
			{
				"site": "twitter",
				"username = "Your Twitter name"
			},
			{
				"site": "facebook",
				"username = "Your Facebook name"
			},
			{
				"site": "github",
				"username = "Your GitHub name"
			},
			{
				"site": "google+",
				"username = "Your Google+ name"
			},
			{
				"site": "linkedin",
				"username = "Your LinkedIn name"
			}
		]
	},
	
	"googleAnalyticsUserID": "Your Optional Analytics User Id",

	"permalinks": {
		"post": "/:year/:month/:day/:filename/"
	}
}
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
