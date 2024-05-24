# eporner-scraper

A bash script for archiving eporner videos, pornstars and playlists metadata in json.

## Requirements

 - [reliq](https://github.com/TUVIMEN/reliq)
 - [jq](https://github.com/stedolan/jq)

## Installation

    install -m 755 eporner-scraper /usr/bin

## Json format

Here's example of a [video](video-example.json), [pornstar](pornstar-example.json) and [playlist](playlist-example.json).

## Usage

Results will be saved in files named by their sha256 hash of urls and placed in DIR.

Download metadata of all videos

    eporner-scraper -v

Download metadata of all playlists using 8 threads

    eporner-scraper -t 8 -P

Download metadata of all pornstars into DIR directory

    eporner-scraper -d DIR -p

Download metadata from URL

    eporner-scraper URL
