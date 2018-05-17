# happypanda
### Script to download galleries from sad panda

## Requires

wget, grep, sed, and optionally zip

You will need a [Netscape style cookie](http://www.cookiecentral.com/faq/#3.5) placed in `~/.exhentai.cookie` in order for this script to work.

## Usage
```
happypanda [URL]
-c |--cookies (cookies file)    Specifies the cookies file
-d |--digits  (number)          Specifies the number of digits in filenames
-z |--zip                       Zip up files
-s |--skip                      Skip existing files
-S |--skip-dirs                 Skip existing directories
-n |--limit (number)            Number of galleries to download ( 0 = unlimited )
-t |--tags (tag)                Download galleries that match the tags ( URL overrides this )
-m |--no-metadata               Do not create a metadata file
   |--doujinshi                 Apply the doujinshi filter
   |--manga                     Apply the manga filter
   |--artist-cg                 Apply the artist cg filter
   |--game-cg                   Apply the game cg filter
   |--western                   Apply the western filter
   |--non-h                     Apply the non-h filter
   |--image-set                 Apply the image set filter
   |--cosplay                   Apply the cosplay filter
   |--asian-porn                Apply the asian porn filter
   |--misc                      Apply the misc filter
```

## Features

Specify a gallery URL to download that single gallery, or specify filters and tags to download all galleries that match. 

If the script is halted, either due to exceeded bandwidth or manually terminating the script, a hidden file will be created that allows the download to resume from where it stopped.
