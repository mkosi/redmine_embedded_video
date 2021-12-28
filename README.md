redmine_embedded_video
======================

Author: Jan Pilz  (see http://www.redmine.org/issues/5171)

Tested redmine 4.2.1

- git clone into redmine to plugins directory
- rake redmine:plugins:migrate RAILS_ENV=production
- restart redmine

Usage:

* `{{video(<ATTACHEMENT>|<URL>|<YOUTUBE_URL>[,<width>,<height>])}}`

For external urls just use the complete http url to the video:
* `{{video(http://youtu.be/o9aA9wCQ9co)}}`
 
You can fore video width and height:
* `{{video(http://youtu.be/o9aA9wCQ9co[640,480])}}`

For relative scale just enter one value:
* `{{video(http://youtu.be/o9aA9wCQ9co[640,])}}`


For attached videos, don't use any path in front of attachment filename
* `{{video(History.flv)}}`
* `{{video(vid.swf)}}`


